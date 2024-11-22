# Projeto: Extração de Dados de Catálogo Online de Motos

## Descrição
Este projeto tem como objetivo entrar em uma página web (catálogo online), esperar o cliente escolher a moto desejada e, em seguida, entrar nos catálogos da moto escolhida, extrair os dados e salvar em um arquivo CSV. O formato dos arquivos está em **Notebook Jupyter**.

## Bibliotecas Utilizadas
- **selenium**: Automação de navegadores web
- **bs4 (BeautifulSoup)**: Análise de documentos HTML e XML
- **time**: Funções de tempo e controle de pausa
- **credenciais**: Arquivo criado para armazenar informações sensíveis, como credenciais de login
- **tkinter**: Criação de interfaces gráficas para o usuário
- **pandas**: Manipulação e análise de dados
- **os**: Interação com o sistema operacional

## Instruções de Uso
1. **Configuração do Ambiente Virtual**:
   - Certifique-se de ter um ambiente virtual configurado para o projeto:
     ```bash
     python -m venv meu_ambiente
     source meu_ambiente/bin/activate  # MacOS/Linux
     meu_ambiente\Scripts\activate     # Windows
     ```

2. **Instalação das Dependências**:
   - Instale as bibliotecas necessárias:
     ```bash
     pip install selenium bs4 pandas tkinter
     ```
   - Crie um arquivo "credenciais.py" e passe dentro dele as informações:
     ```bash
     credenciais = {
        'CPF': 'xxxxxxxxxxx',
        'CPF_FORMATADO': 'xxx.xxx.xxx-xx',
        'SENHA': 'sua_senha',
        'PAGINA_WEB': 'página_do_portal'
     }
     ```

3. **Execução do Script**:
   - Abra o Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Execute o script no Notebook, seguindo as instruções para selecionar a moto desejada e extrair os dados.

## Estrutura do Projeto
- **catalogo_online.ipynb**: Notebook Jupyter contendo o script principal.
- **credenciais.py**: Arquivo contendo funções para gerenciamento de credenciais.
- **data/**: Diretório para salvar os arquivos CSV gerados.

## Exemplos de Uso
Dentro do Notebook Jupyter, a execução do script envolverá passos como:
1. Entrar na página do catálogo online.
2. Esperar o cliente escolher a moto desejada.
3. Entrar nos catálogos da moto escolhida.
4. Extrair os dados específicos.
5. Salvar os dados extraídos em um arquivo CSV.

## Observações
- Certifique-se de ajustar as configurações do WebDriver do Selenium conforme necessário para seu navegador.
- Este projeto requer conexão com a internet para acessar os catálogos online.

## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

