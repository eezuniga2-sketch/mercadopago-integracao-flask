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
