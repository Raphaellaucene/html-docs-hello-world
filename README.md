# Objetivo

- Descrever os principais componentes e valores do Serviço de Aplicativos do Azure.
- Explicar como o Serviço de Aplicativo do Azure gerencia a autenticação e a autorização.
- Identificar métodos para controlar o tráfego de entrada e saída para seu aplicativo Web.
- Implantar um aplicativo no Serviço de Aplicativo usando os comandos da CLI do Azure.

# Requisitos:

 - Pelo menos 6 meses de expeiência no desenvolvimento de soluções escalonáveis em todas as fases do desenvolvimento de software.
 - Ter uma compreensão básica do Azure e dos conceitos de nuvem, serviços e portal Azure.
 - Conhecimentos básicos em C#, .Net Framework, HTML e uso de REST em aplictivos.
 - Familiaridade com a CLI do Azure e/ou PowerShell.

---

# Introdução Serviço de Aplicativo do Azure

- O Serviço de Aplicativo do Azure é um serviço com base em HTTP para hospedagem de aplicativos Web, API's REST e back-ends móveis.
- Os aplicativos são executados e dimensionados em ambientes baseados no Window e Linux.

## Comandos Azure CLI no CMD

1. Conecte-se a sua assinatura Azure:
    ```sh
    az login
    ```
2. Listar grupos de recursos:
    ```sh
    az group list --query "[].{id:name}" -o tsv
    ```
3. Criar o aplicativo e subir atualizações:
    ```sh
    az webapp up -g <grupoderecurso> -n <nomeapp> --html
    ```
4. Obter log stream:
    ```sh
    az webapp log tail --name <nomeapp> --resource-group <grupoderecurso>
    ```

---

# Configurações do Aplicativo Web

- Configurações de aplicativos associadas aos slots de implantação
- Opções de instalação de certificados TLS para seu app
- Log de diagnóstico para seu aplicativo para auxiliar no monitoramento e na depuração
- Aplicativo virtual para mapeamentos de diretório

---

# Dimensionameto Automático

- Identificar cenários em que o dimensionamento automático é uma solução adequada
- Regras de dimensionamento para um web app
- Monitorar os efeitos do dimensionamento automático

---

# Readme Sample

topic: HTML Hello World
languages:
  - HTML
products:
  - Azure App Service
  - Azure Web Apps

# HTML Hello World

This sample demonstrates a tiny Hello World HTML app for [App Service](https://docs.microsoft.com/azure/app-service).

# Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.