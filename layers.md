### index.js 

Responsável por chamar todas as camadas

### workers -> processo em segundo plano

* Toda lógica PESADA (que envolve CPU)
* Tudo que possa travar a tela (for loop, machine learning, AI, processamento de CAM)

### services
* toda lógica de negócio
* toda chamada externa (API, arquivos, banco de dados)

### views  

Toda interação com o DOM (com HTML, com a página)

### controllers -> é a intermediaria entre services e/ou workers e views

### factories
* a factory é quem importa as dependecias 
* e cria o objeto final para fazermos as chamadas
* retorna a função que inicializa o fluxo daquele componente (init)
