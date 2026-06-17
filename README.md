# final-proyect
My ultimo projecto de pyton pro
VISION POR ORDENADOR
from flask import Flask, render_template

app = Flask(__name__)


@app.route("/")
def inicio():
    return render_template("inicio.html")


@app.route("/clasificador")
def clasificador():
    return render_template("clasificador.html")


if __name__ == "__main__":
    app.run(debug=True)
