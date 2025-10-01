## Exemplo técnico da aplicação Flask

A seguir, apresentamos dois fragmentos simulados que representam a estrutura básica de uma aplicação Flask voltada para um Marketplace de produtos artesanais. Esses exemplos foram incluídos com fins acadêmicos para evidenciar a organização técnica e semântica do projeto.

### 📄 app.py

```python
# Importa o framework Flask
from flask import Flask, render_template

# Cria a aplicação
app = Flask(__name__)

# Rota principal que renderiza a página inicial
@app.route('/')
def home():
    return render_template('index.html')  # Página com produtos artesanais

# Executa a aplicação localmente
if __name__ == '__main__':
    app.run(debug=True)
## Ejemplo de estructura HTML (index.html)

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Tienda Artesanal</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body { font-family: sans-serif; margin: 2rem; background-color: #f4f4f4; }
    header { text-align: center; margin-bottom: 2rem; }
    section { display: flex; gap: 2rem; flex-wrap: wrap; }
    article { background: white; padding: 1rem; border-radius: 8px; box-shadow: 0 0 5px rgba(0,0,0,0.1); width: 300px; }
    button { background-color: #28a745; color: white; border: none; padding: 0.5rem 1rem; border-radius: 4px; cursor: pointer; }
  </style>
</head>
<body>
  <header>
    <h1>Productos Artesanales</h1>
    <p>Explora nuestra selección hecha a mano con dedicación.</p>
  </header>
  <main>
    <section>
      <article>
        <h2>Jabón Natural</h2>
        <p>Elaborado con aceites esenciales y ingredientes orgánicos.</p>
        <button>Comprar</button>
      </article>
      <article>
        <h2>Velas Aromáticas</h2>
        <p>Hechas a mano, con fragancias suaves y relajantes.</p>
        <button>Comprar</button>
      </article>
    </section>
  </main>
</body>
</html>
