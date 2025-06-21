Portal Bíblico
Um portal interativo para explorar a história bíblica com slides, mapas e uma linha do tempo. Construído com React, Vite, Tailwind CSS, Swiper, Leaflet e um backend Node.js com Express.
Sobre o Projeto
O Portal Bíblico é uma aplicação web que oferece uma experiência educacional para explorar eventos, locais e períodos da história bíblica. Suas principais funcionalidades incluem:

Slides Interativos: Apresenta eventos bíblicos com imagens e descrições usando o Swiper.
Mapas Interativos: Exibe locais bíblicos em um mapa com Leaflet, com marcadores e pop-ups.
Linha do Tempo: Organiza eventos históricos em períodos cronológicos, consumindo dados de uma API.
Design Responsivo: Interface estilizada com Tailwind CSS, adaptável a dispositivos móveis e desktops.

O frontend é construído com React e Vite, enquanto o backend usa Node.js com Express para fornecer dados via API.
Tecnologias Utilizadas

Frontend:
React 18
Vite 5
Tailwind CSS 3
Swiper 9
Leaflet 1.9


Backend:
Node.js
Express
CORS


Outras Ferramentas:
PostCSS
Autoprefixer



Pré-requisitos

Node.js v16 ou superior
npm v8 ou superior
Um navegador moderno (Chrome, Firefox, Edge, etc.)

Instalação

Clone o repositório:
git clone https://github.com/abnerpp/PortalBiblico.git
cd PortalBiblico


Instale as dependências do frontend:
cd client
npm install


Instale as dependências do backend:
cd ../server
npm install


Configure os arquivos de dados:

Verifique que server/data/timeline.json e server/data/maps.json existem e contêm os dados necessários.
Exemplo de estrutura para timeline.json:{
  "periods": [
    {
      "title": "Período Patriarcal",
      "startYear": "2000 a.C.",
      "endYear": "1500 a.C.",
      "events": [
        { "year": "2000 a.C.", "description": "Chamada de Abraão (Gênesis 12)" }
      ]
    }
  ]
}




Inicie o backend:
cd server
node server.js

O servidor estará rodando em http://localhost:3000.

Inicie o frontend em modo de desenvolvimento:
cd ../client
npm run dev

O frontend estará disponível em http://localhost:5173.

(Opcional) Crie o build do frontend para produção:
npm run build

Os arquivos de build estarão em client/dist/. O backend servirá esses arquivos automaticamente em http://localhost:3000.


Uso

Navegação: Use a barra de navegação para alternar entre Slides, Mapas e Linha do Tempo.
Slides: Navegue pelos slides com as setas ou a paginação do Swiper.
Mapas: Clique nos marcadores para ver detalhes sobre locais bíblicos.
Linha do Tempo: Explore eventos organizados por períodos históricos.
Acesse http://localhost:3000 após iniciar o backend para ver a aplicação completa.

Estrutura do Projeto
PortalBiblico/
├── client/                   # Frontend (React + Vite)
│   ├── public/               # Arquivos públicos (opcional)
│   ├── src/                  # Código-fonte do frontend
│   │   ├── components/       # Componentes React (Navigation, Slide, MapViewer, Timeline)
│   │   ├── styles/           # Estilos (index.css com Tailwind)
│   │   ├── App.jsx           # Componente principal
│   │   └── main.jsx          # Ponto de entrada do React
│   ├── index.html            # Página HTML principal
│   ├── package.json          # Dependências e scripts do frontend
│   ├── vite.config.js        # Configuração do Vite
│   ├── tailwind.config.js    # Configuração do Tailwind CSS
│   └── postcss.config.js     # Configuração do PostCSS
├── server/                   # Backend (Node.js + Express)
│   ├── data/                 # Arquivos JSON (timeline.json, maps.json)
│   ├── routes/               # Rotas da API (api.js)
│   ├── server.js             # Servidor Express
│   └── package.json          # Dependências e scripts do backend
└── README.md                 # Documentação do projeto

Contribuição

Faça um fork do repositório.
Crie uma branch para sua feature:git checkout -b minha-feature


Commit suas alterações:git commit -m "Adiciona minha feature"


Push para a branch:git push origin minha-feature


Abra um Pull Request.

Licença
Este projeto está licenciado sob a MIT License.
Contato
Para dúvidas ou sugestões, entre em contato via arierap@gmail.com ou abra uma issue no GitHub.
