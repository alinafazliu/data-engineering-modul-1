# Setup

## For students — Google Colab (recommended, nothing to install)

1. Sign in to Google with any account and open <https://colab.research.google.com>.
2. *File → Open notebook → GitHub*, paste the course repository URL (your teacher shares it) and pick the notebook for today's session.
3. Run the first code cell. It downloads the course data into Colab (takes a few seconds).
4. From session 3 on, the second cell starts Spark (about 20–30 seconds the first time).
5. To keep your work: *File → Save a copy in Drive* (or *Save a copy in GitHub*, see session 6).

Colab forgets all files when the runtime stops. That is fine: every notebook downloads or rebuilds what it needs.

## Optional — run locally (for experienced students)

You need **Python 3.10–3.12** and **Java 17** (Spark runs on the Java Virtual Machine).

```bash
git clone https://github.com/alinafazliu/data-engineering-modul-1.git
cd <repository>
python -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

Check Java with `java -version`. On Windows, Spark also needs extra Hadoop files (`winutils.exe`) to write files, so Colab is much easier there.
