---
title: Instalar um SDK do Microsoft Graph
description: Encontre instruções para instalar os SDKs do Microsoft Graph para .NET, Go, Java, JavaScript, PHP, PowerShell e Python.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 7d1192b54736958858848084ae4786ef946f4c11
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577599"
---
# <a name="install-a-microsoft-graph-sdk"></a>Instalar um SDK do Microsoft Graph

Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio do GitHub e de gerenciadores de pacotes de plataforma populares. Este artigo descreve como você pode instalar um SDK do Microsoft Graph em seu projeto.

Os SDKs estão disponíveis nos seguintes idiomas:

- [.NET](#install-the-microsoft-graph-net-sdk)
- [Go (versão prévia)](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (versão prévia)](#install-the-microsoft-graph-python-sdk-preview)

## <a name="install-the-microsoft-graph-net-sdk"></a>Instalar o SDK do .NET do Microsoft Graph

O SDK do .NET do Microsoft Graph está incluído nos seguintes pacotes NuGet:

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet): contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente. O Microsoft.Graph tem uma dependência no Microsoft.Graph.Core.
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet): contém os modelos e os construtores de solicitação para acessar o ponto `beta` de extremidade com a API fluente. O Microsoft.Graph.Beta tem uma dependência no Microsoft.Graph.Core.
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet): a biblioteca principal para fazer chamadas ao Microsoft Graph.

Para instalar os pacotes do Microsoft.Graph em seu projeto, você pode usar a interface do usuário do Gerenciador de Pacotes no [Visual Studio ou o Console do Gerenciador de Pacotes](/nuget/quickstart/install-and-use-a-package-in-visual-studio). Os comandos do Console do Gerenciador de Pacotes a seguir instalam as bibliotecas Microsoft.Graph e Microsoft.Graph.Core. O Microsoft.Graph.Core é instalado como uma dependência do Microsoft.Graph.

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>Instalar o SDK do Microsoft Graph Go (versão prévia)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

O SDK do Microsoft Graph Go está incluído nos seguintes pacotes:

- [SDK do Microsoft Graph para Go](https://github.com/microsoftgraph/msgraph-sdk-go): contém os modelos e os construtores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente.
- [SDK Beta do Microsoft Graph para Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go): contém os modelos `beta` e os construtores de solicitação para acessar o ponto de extremidade com a API fluente.
- [SDK principal do Microsoft Graph para Go](https://github.com/microsoftgraph/msgraph-sdk-go-core): a biblioteca principal para fazer chamadas ao Microsoft Graph.

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Instalar o SDK do Java do Microsoft Graph

O SDK do Java do Microsoft Graph está incluído nos seguintes pacotes:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java): contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java): contém os modelos e os construtores de solicitação para acessar o ponto `beta` de extremidade com a API fluente.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core): a biblioteca principal para fazer chamadas ao Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth): fornece um wrapper baseado em cenário de autenticação da MSAL (Biblioteca de Autenticação da Microsoft) para uso com o SDK do Microsoft Graph.

Para instalar o SDK do Java do Microsoft Graph, siga um dos seguintes procedimentos:

- Use o Gradle para instalar o SDK do Java do Microsoft Graph. Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do projeto:
    
  ```Gradle
    repository {
        mavenCentral()
    }
    
    dependency {
        // Include the sdk as a dependency
        implementation 'com.microsoft.graph:microsoft-graph:5.+'
        // Include Azure identity for authentication
        implementation 'com.azure:azure-identity:1.+'
    }
  ```

- Use o Maven para instalar o SDK do Java do Microsoft Graph. Adicione a dependência no elemento `dependencies` em pom.xml:
    
  ```xml
    <dependency>
        <groupId>com.microsoft.graph</groupId>
        <artifactId>microsoft-graph</artifactId>
        <version>[5.0,)</version>
    </dependency>
    <dependency>
        <groupId>com.azure</groupId>
        <artifactId>azure-identity</artifactId>
        <version>[1.3,)</version>
    </dependency>
  ```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o SDK do JavaScript do Microsoft Graph

O SDK javaScript do Microsoft Graph está incluído nos seguintes pacotes:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)): a biblioteca principal para fazer chamadas ao Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)): os tipos TypeScript para as entidades do Microsoft Graph.

Use [npm](https://www.npmjs.com) para instalar o SDK javaScript do Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Instalar o SDK do PHP do Microsoft Graph

O [SDK do PHP do Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível [packagist.org e pode](https://packagist.org/packages/microsoft/microsoft-graph) ser instalado das seguintes maneiras:

- Use o composer para instalar o SDK do PHP do Microsoft Graph manualmente:

    ```Shell
    composer require microsoft/microsoft-graph
    ```

- Use composer.json para instalar o SDK do PHP do Microsoft Graph:

    ```json
    {
        "require": {
            "microsoft/microsoft-graph": "^1.8"
        }
    }
    ```

## <a name="install-the-microsoft-graph-powershell-sdk"></a>Instalar o SDK do PowerShell do Microsoft Graph

Todos os módulos são publicados [Galeria do PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph). Para instalar:

``` powershell
Install-Module Microsoft.Graph
```

Se você estiver atualizando dos módulos de visualização, execute `Install-Module` com `AllowClobber` `Force` parâmetros para evitar conflitos de nome de comando:

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>Instalar o SDK do Python do Microsoft Graph (versão prévia)

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

A [Biblioteca de Clientes python principal do Microsoft Graph (versão prévia)](https://github.com/microsoftgraph/msgraph-sdk-python-core) está disponível no [PyPI](https://pypi.org/).

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```

## <a name="see-also"></a>Confira também

- Para obter mais detalhes sobre os recursos e as funcionalidades do SDK, consulte a documentação de requisitos de [design do](https://github.com/microsoftgraph/msgraph-sdk-design) SDK. 
- Para obter uma lista de exemplos do Microsoft Graph, consulte a página de [recursos do Microsoft Graph](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples).
- Para obter treinamento passo a passo para criar um aplicativo do Microsoft Graph, consulte os [tutoriais do Microsoft Graph](/graph/tutorials).