# BookConnect

Aplicativo desenvolvido em parceria com a **CIA do Livro** para a disciplina de desenvolvimento mobile.  
Nosso objetivo é criar uma plataforma que conecte a livraria e seus clientes com uma experiência moderna, rápida e acessível.



# Objetivo

Estabelecer vínculos entre a livraria e os leitores, permitindo:
- Visualização de livros por categorias
- Detalhes e recomendações personalizadas
- Carrinho de compras e histórico de pedidos
- Login e perfil do usuário


## 🧱 Estrutura do Projeto

📂 `/docs/`
- `fluxo-navegacao.pdf`: (import graphviz

# Criar o fluxograma de navegação do aplicativo BookConnect
fluxo = graphviz.Digraph(format='png')
fluxo.attr(rankdir='LR', size='10')

# Telas principais
fluxo.node('Splash', 'Splash (Inicial)')
fluxo.node('Login', 'Login/Cadastro')
fluxo.node('Home', 'Home (Destaques)')
fluxo.node('Categorias', 'Categorias de Livros')
fluxo.node('Detalhes', 'Detalhe do Livro')
fluxo.node('Buscar', 'Busca')
fluxo.node('Favoritos', 'Favoritos')
fluxo.node('Carrinho', 'Carrinho de Compras')
fluxo.node('Checkout', 'Finalizar Compra')
fluxo.node('Perfil', 'Perfil do Usuário')
fluxo.node('Historico', 'Histórico de Pedidos')

# Conexões entre as telas
fluxo.edges([
    ('Splash', 'Login'),
    ('Login', 'Home'),
    ('Home', 'Categorias'),
    ('Home', 'Buscar'),
    ('Home', 'Favoritos'),
    ('Home', 'Perfil'),
    ('Categorias', 'Detalhes'),
    ('Buscar', 'Detalhes'),
    ('Favoritos', 'Detalhes'),
    ('Detalhes', 'Carrinho'),
    ('Carrinho', 'Checkout'),
    ('Perfil', 'Historico')
])

fluxo.render('fluxograma_bookconnect', cleanup=False)
)  
- `arquitetura-app.pdf`: Arquitetura e divisão lógica  
- `telas/`: Imagens com os layouts das telas

📂 `/prototype/`
- Arquivo original Figma (opcional, `.fig`)

---

# Protótipo no Figma

👉 [Acesse o protótipo do BookConnect no Figma (clique aqui)](https://www.figma.com/design/1iF5VWKa3iyu6izd71kbv2/Sem-t%C3%ADtulo?node-id=0-1&m=dev&t=nQY2YYlAJPEGS6GE-1))



# Tecnologias previstas para a próxima fase

- React Native (ou Flutter)
- Firebase (autenticação, banco de dados e storage)
- Styled Components
- Context API (ou Redux)

---

#  Integrantes do Grupo

- Nome 1 — Naamã
- Nome 2 — Washingtom
- Nome 3 — Otavio 


---

## 📅 Entrega - Parte 1

✅ Estrutura do app  
✅ Protótipo no Figma  
✅ Fluxo de navegação  
✅ Repositório público com versionamento no GitHub

---



