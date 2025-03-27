# Verificador de Sites - Segurança e Status Online 🌐

## Sobre o Projeto
O **Verificador de Sites** é um aplicativo que permite checar rapidamente o status de um site (se está online ou offline) e verificar sua segurança utilizando a API do Google Safe Browsing. 

Este projeto foi desenvolvido como parte do meu aprendizado em **Segurança da Informação** e **Desenvolvimento Python**, aplicando conceitos como requisições HTTP, manipulação de APIs, interface gráfica (Tkinter) e registro de logs.

## Funcionalidades ✅
- **Verificação de Status**: Confere se um site está online ou offline.
- **Verificação de Segurança**: Analisa se o site é considerado malicioso ou suspeito.
- **Registro de Logs**: Todos os resultados das verificações são armazenados para consulta posterior.
- **Interface Personalizada**: Design temático espacial para uma experiência diferenciada.
- **Opção de Apagar Logs**: Permite limpar os registros quando necessário.

## Como Funciona 🛠️
### 1️⃣ Verificação de Status
O programa faz uma requisição HTTP para o site informado e analisa o código de resposta:
- **200**: O site está online ✅
- **Outros códigos**: O site pode estar com problemas ⚠️
- **Sem resposta**: O site está offline ❌

### 2️⃣ Verificação de Segurança
O sistema consulta a API do **Google Safe Browsing**, que contém uma lista atualizada de sites perigosos (phishing, malware, etc.). Caso o site esteja na lista, um alerta será exibido.

### 3️⃣ Registro de Logs
Todas as verificações são salvas no arquivo `verificador_logs.txt`, contendo a data, hora e o resultado.

### 4️⃣ Exclusão de Logs
Para evitar acúmulo de arquivos, há um botão que permite excluir os logs antigos.

## Como Usar 🚀
### 1. Configurar a Chave de API do Google Safe Browsing
Para usar a verificação de segurança, é necessário gerar uma **API Key** do Google:
- Acesse [Google Cloud Console](https://console.cloud.google.com/)
- Crie um novo projeto e ative a API Safe Browsing
- Gere uma **API Key** e substitua `SUA_CHAVE_AQUI` no código.

### 2. Instalar Dependências
Antes de rodar o programa, instale as bibliotecas necessárias:
```sh
pip install requests
```

### 3. Executar o Programa
Salve o código como `verificador.py` e execute:
```sh
python verificador.py
```

## Tecnologias Utilizadas 🛠️
- **Python**: Linguagem principal do projeto
- **Tkinter**: Interface gráfica
- **Requests**: Requisições HTTP
- **Google Safe Browsing API**: Verificação de segurança


## Sobre Mim 👨‍💻
Este projeto foi desenvolvido por **Vinicius Ribeiro** como parte do meu aprendizado na área de **Segurança da Informação**. 

Conecte-se comigo no [LinkedIn](https://www.linkedin.com/in/euvinil/).

