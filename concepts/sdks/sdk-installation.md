---
title: Instalar o SDK do Microsoft Graph
description: Fornece instruções para a instalação dos SDKs C#, Java, JavaScript, Objective-C, PHP e Ruby do Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: a46f005e2ff646f420d19741eca3c8c21a95291a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630178"
---
# <a name="install-the-microsoft-graph-sdks"></a>Instalar os SDKs do Microsoft Graph

Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio do GitHub e gerentes de pacotes de plataforma populares. Este tópico descreve como você pode instalar o SDK do Microsoft Graph em seu projeto.

## <a name="install-the-microsoft-graph-net-sdk"></a>Instalar o SDK do Microsoft Graph .NET

O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:

* [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -contém os modelos e criadores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente. O Microsoft. Graph tem uma dependência em Microsoft. Graph. Core.
* [Microsoft. Graph. beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -contém os modelos e criadores de solicitação para acessar o `beta` ponto de extremidade com a API fluente. Microsoft. Graph. beta tem uma dependência em Microsoft. Graph. Core.
* [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -a biblioteca principal para fazer chamadas para o Microsoft Graph.
* [Microsoft. Graph. auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) : fornece um wrapper baseado em cenário de autenticação da biblioteca de autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph. Microsoft. Graph. auth tem uma dependência em Microsoft. Graph. Core.

Você pode usar a [interface do usuário do Gerenciador de pacotes no Visual Studio ou no console do Gerenciador de pacotes](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio) para instalar os pacotes do Microsoft. Graph em seu projeto. Os seguintes comandos do console do Gerenciador de pacotes instalarão as bibliotecas Microsoft. Graph, Microsoft. Graph. Core e Microsoft. Graph. auth. O Microsoft. Graph. Core é instalado como uma dependência de Microsoft. Graph.

```
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Instalar o SDK do Microsoft Graph Java

O SDK do Microsoft Graph Java está incluído nos seguintes pacotes:

* [Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) -contém os modelos e criadores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente.
* [Microsoft-Graph-Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -a biblioteca principal para fazer chamadas para o Microsoft Graph.
* [Microsoft-Graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -fornece um wrapper baseado em cenário de autenticação da biblioteca de autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Instalar o SDK do Microsoft Graph Java via gradle

Adicione o repositório e uma dependência de compilação do Microsoft-Graph à compilação do seu projeto. gradle:

```
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Instalar o SDK do Microsoft Graph Java via Maven

Adicione a dependência no elemento Dependencies em pom. xml:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o SDK do JavaScript do Microsoft Graph

O SDK do JavaScript do Microsoft Graph está incluído nos seguintes pacotes:

* @microsoft/Microsoft-Graph-Client ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))-a biblioteca principal para fazer chamadas para o Microsoft Graph.
* @microsoft/Microsoft-Graph-Types ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-types))-os tipos de typescript para entidades do Microsoft Graph.

Você pode usar o [NPM](https://www.npmjs.com) para instalar o SDK do JavaScript do Microsoft Graph:

```
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Instalar o SDK do Microsoft Graph objetivo-C

O SDK do Microsoft Graph objetivo-C suporta as plataformas iOS e macOS e pode ser instalado em seu projeto usando o CocoaPods ou o Carthage.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Instale o SDK do Microsoft Graph objetivo-C usando Cocoapods

Adicione a seguinte linha no seu podfile para incluir o SDK do Microsoft Graph objetivo e o SDK do Microsoft Graph objetivo-C de autenticação no seu projeto do Xcode:

```
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Instale o SDK do Microsoft Graph objetivo-C usando Carthage

Execute as seguintes etapas para instalar o Microsoft Graph objector-C SDK e o Microsoft Graph Objective SDK-C auth using the [Carthage](https://github.com/Carthage/Carthage) Package Manager.

1. Crie um **cartfile** que especifica o repositório e a [marca de versão](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) do SDK do

```
github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
```

2. Executar `carthage update`. Isso irá buscar dependências em uma pasta Carthage/checkouts e, em seguida, cria a biblioteca MSGraphClientSDK.

3. Usando o Xcode, na guia configurações **gerais** da sua meta de aplicativo, na seção **estruturas e bibliotecas vinculadas** , arraste e solte o **MSGraphClientSDK. Framework** e o **MSGraphMSALAuthProvider. Framework** do Carthage/ Criar pasta no disco.

4. Na guia Configurações de **fases de compilação** do seu destino de aplicativo **+** , clique no ícone e escolha **nova fase de script de execução**. Crie um script de execução em que você especifique seu shell (ex:/bin/sh) e adicione o seguinte conteúdo ao script:

```
/usr/local/bin/carthage copy-frameworks
```

5. Adicione os caminhos para os frameworks que você deseja usar em **arquivos de entrada**.

```
$(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
$(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
```

## <a name="install-the-microsoft-graph-php-sdk"></a>Instalar o SDK do Microsoft Graph PHP

O [SDK do Microsoft Graph php](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível no [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) e pode ser instalado das seguintes maneiras:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Instalar o SDK do Microsoft Graph PHP manualmente usando o Composer

```
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Instalar o SDK do Microsoft Graph PHP usando o Composer. JSON

```
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Instalar o SDK do Microsoft Graph Ruby

O [SDK do Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) está disponível no [RubyGems.org](https://rubygems.org/) e pode ser instalado usando o seguinte comando:

```
gem install microsoft_graph
```
