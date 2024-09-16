# GrowerTech

GrowerTech é um sistema de recomendação personalizada de insumos agrícolas, desenvolvido para auxiliar produtores rurais a tomar decisões mais assertivas sobre quais insumos utilizar em suas plantações. O sistema utiliza uma análise detalhada de dados agronômicos, como condições climáticas, tipos de solo, histórico de cultivos e outras variáveis, para sugerir os insumos mais adequados para cada cenário.

## Funcionalidades Principais

### 1. Registro de Propriedades Rurais
- **Cadastro de Propriedades**: Os produtores podem cadastrar informações detalhadas sobre suas propriedades, incluindo localização geográfica (coordenadas GPS), tamanho da área cultivada e tipos de cultura.
- **Histórico de Cultivos**: Armazena o histórico de plantios, permitindo a análise de ciclos de produção e a previsão de melhores insumos com base nas safras anteriores.

### 2. Análise de Dados Agronômicos
- **Condições Climáticas**: O sistema coleta dados em tempo real ou históricos de fontes meteorológicas para ajustar as recomendações de insumos de acordo com as previsões de clima, temperatura e níveis de precipitação.
- **Tipos de Solo**: Com base nas amostras de solo fornecidas, o sistema avalia a composição química e mineral para determinar os melhores insumos (fertilizantes, corretivos etc.).
- **Níveis de Umidade e Irrigação**: Monitora os níveis de umidade do solo, recomendando ajustes nos sistemas de irrigação ou adubação conforme necessário.
- **Histórico de Pragas e Doenças**: Integra informações sobre surtos anteriores de pragas e doenças, sugerindo insumos que podem ajudar na prevenção e tratamento.

### 3. Recomendação de Insumos Agrícolas
- **Recomendações Baseadas em Dados**: Com a análise agronômica em mãos, o sistema recomenda insumos específicos, como fertilizantes, pesticidas e herbicidas, ajustados para as condições de cultivo.
- **Integração com Fornecedores**: Possibilidade de integração com fornecedores locais para facilitar a compra dos insumos recomendados, agilizando o processo para o produtor.
- **Relatórios Personalizados**: Gera relatórios com análises detalhadas para cada propriedade, permitindo que o produtor visualize as recomendações e entenda as razões por trás de cada sugestão.

## Tecnologias Utilizadas
- **Front-End**: React.js para a interface do usuário, proporcionando uma experiência intuitiva e responsiva.
- **Back-End**: Java API, responsável pelo processamento de dados e integração com fontes externas de informação climática e agronômica.
- **Banco de Dados**: Oracle para armazenar informações das propriedades, histórico de cultivos e dados de insumos recomendados.
- **Machine Learning**: Modelos de aprendizado de máquina para análise preditiva, utilizando bibliotecas como Scikit-learn ou TensorFlow para otimizar as recomendações.
- **Integração de APIs Climáticas**: Conectividade com APIs como OpenWeather para obter dados climáticos precisos em tempo real.
- **Mapeamento Geoespacial**: Google Maps API para registro e visualização das propriedades agrícolas no mapa.

## Como Funciona

1. **Cadastro**: O produtor se registra na plataforma e insere informações sobre sua propriedade e tipo de cultura.
2. **Coleta de Dados**: O sistema coleta dados agronômicos automaticamente através de APIs, sensores conectados (IoT) ou entrada manual pelo usuário.
3. **Análise e Recomendação**: Utilizando algoritmos de aprendizado de máquina e dados agronômicos, o GrowerTech faz a recomendação dos melhores insumos para cada situação específica.
4. **Relatórios e Ações**: O usuário recebe relatórios detalhados com as recomendações e pode tomar decisões informadas sobre quais insumos adquirir e utilizar.

## Configuração do Ambiente de Desenvolvimento

Para rodar o projeto localmente, siga os passos abaixo:

### Pré-requisitos
- JAVA (versão 17)
- Oracle
- Git
- API Key do OpenWeather (opcional para funcionalidades climáticas)

### Instalação

1. Clone o repositório:
    ```bash
    git clone https://github.com/MunirAyoub/growertech.git
    cd growertech
    ```

2. Instale as dependências:
    ```bash
    npm install
    ```

3. Configure o banco de dados e as variáveis de ambiente:
    - Crie um arquivo `.env` e adicione as seguintes variáveis:
        ```
        DB_HOST=localhost
        DB_USER=seuusuario
        DB_PASS=suasenha
        DB_NAME=growertech
        OPENWEATHER_API_KEY=sua_api_key
        ```

4. Execute o servidor:
    ```bash
    npm run dev
    ```

5. Acesse a aplicação no navegador através do endereço:
    ```
    http://localhost:8080
    ```

