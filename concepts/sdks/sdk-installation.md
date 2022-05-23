---
title: Instalar um SDK do Microsoft Graph
description: Fornece instruções para instalar os SDKs do Microsoft Graph .NET, Go, Java, JavaScript, PHP, PowerShell e Python.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 659730d111e3d23f0ef7a9d9352a5dc6730e37c3
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628696"
---
# <a name="install-a-microsoft-graph-sdk"></a>Instalar um SDK do Microsoft Graph

Os SDKs Graph Microsoft estão disponíveis para vários idiomas a serem incluídos em seus projetos por meio de GitHub e gerenciadores de pacotes de plataforma populares. Este artigo descreve como você pode instalar um Microsoft Graph SDK em seu projeto.

Os SDKs estão disponíveis nos idiomas a seguir.

- [.NET](#install-the-microsoft-graph-net-sdk)
- [Go (versão prévia)](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (versão prévia)](#install-the-microsoft-graph-python-sdk-preview)

## <a name="install-the-microsoft-graph-net-sdk"></a>Instalar o SDK do .NET Graph Microsoft Graph

O Microsoft Graph SDK do .NET está incluído nos seguintes NuGet pacotes:

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente. Microsoft. Graph tem uma dependência da Microsoft. Graph. Núcleo.
- [Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) – Contém os modelos e os construtores de solicitação para acessar o ponto `beta` de extremidade com a API fluente. Microsoft. Graph. Beta tem uma dependência da Microsoft. Graph. Núcleo.
- [Microsoft. Graph. Núcleo](https://github.com/microsoftgraph/msgraph-sdk-dotnet) – a biblioteca principal para fazer chamadas para o Microsoft Graph.

Você pode usar a interface [do usuário Gerenciador de Pacotes no Visual Studio ou o Console do Gerenciador de Pacotes](/nuget/quickstart/install-and-use-a-package-in-visual-studio) para instalar os pacotes microsoft.Graph em seu projeto. Os comandos Gerenciador de Pacotes Console a seguir instalarão o Microsoft.Graph e o Microsoft.Graph. Bibliotecas principais. Microsoft. Graph. O Core é instalado como uma dependência da Microsoft. Graph.

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>Instalar o SDK do Microsoft Graph Go (versão prévia)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

O SDK do Microsoft Graph Go está incluído nos seguintes pacotes:

- [Microsoft Graph SDK para Go](https://github.com/microsoftgraph/msgraph-sdk-go) – `v1.0` Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade com a API fluente.
- [Microsoft Graph SDK Beta para Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go) – `beta` Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade com a API fluente.
- [Microsoft Graph Core SDK para Go](https://github.com/microsoftgraph/msgraph-sdk-go-core) – a biblioteca principal para fazer chamadas para o Microsoft Graph.

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Instalar o Microsoft Graph Java SDK

O Microsoft Graph Java SDK está incluído nos seguintes pacotes:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) – contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) – contém os modelos e os construtores de solicitação para acessar o ponto `beta` de extremidade com a API fluente.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) – a biblioteca principal para fazer chamadas para o Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) – fornece um wrapper baseado em cenário de autenticação da MSAL (Biblioteca de Autenticação da Microsoft) para uso com o Microsoft Graph SDK.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Instalar o SDK do Java do Microsoft Graph via Gradle

Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do projeto:

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

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Instalar o SDK do Java do Microsoft Graph via Maven

Adicione a dependência no elemento `dependencies` em pom.xml:

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o SDK do Microsoft Graph JavaScript

O SDK do Microsoft Graph JavaScript está incluído nos seguintes pacotes:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) – a biblioteca principal para fazer chamadas para o Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) – os tipos Typescript para as entidades do Microsoft Graph.

Você pode usar [npm](https://www.npmjs.com) para instalar o SDK Graph JavaScript do Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Instalar o Microsoft Graph PHP SDK

O [Microsoft Graph SDK do PHP](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível packagist.org e pode ser [](https://packagist.org/packages/microsoft/microsoft-graph) instalado das seguintes maneiras:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Instalar o SDK do PHP do Microsoft Graph manualmente usando o composer

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Instalar o SDK do PHP do Microsoft Graph usando composer.json

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-powershell-sdk"></a>Instalar o SDK do Microsoft Graph PowerShell

Todos os módulos são publicados [Galeria do PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph). Para instalar:

``` powershell
Install-Module Microsoft.Graph
```

Se você estiver atualizando dos módulos de visualização, `Install-Module` execute com os parâmetros AllowClobber e Force para evitar conflitos de nome de comando:

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>Instalar o SDK do Python do Microsoft Graph (versão prévia)

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

O [Microsoft Graph Core Python Client Library (versão prévia)](https://github.com/microsoftgraph/msgraph-sdk-python-core) está disponível no [PyPI](https://pypi.org/).

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```
