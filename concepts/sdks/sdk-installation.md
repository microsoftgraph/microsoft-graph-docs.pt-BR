---
title: Instalar o SDK do Microsoft Graph
description: Fornece instruções para instalar os C#, Java, Javascript, Objective-C, PHP e Ruby Microsoft Graph SDKs.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: cd019a8f13bd0ffe154a2a998d59815addf664e9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941390"
---
# <a name="install-the-microsoft-graph-sdks"></a>Instalar os SDKs do Microsoft Graph

Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio do GitHub e gerentes de pacotes de plataforma populares. Este tópico descreve como você pode instalar o SDK do Microsoft Graph em seu projeto.

## <a name="install-the-microsoft-graph-net-sdk"></a>Instalar o SDK do Microsoft Graph .NET

O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente. O Microsoft.Graph tem uma dependência do Microsoft.Graph.Core.
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade `beta` com a API fluente. O Microsoft.Graph.Beta tem uma dependência do Microsoft.Graph.Core.
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - A biblioteca principal para fazer chamadas para o Microsoft Graph.
- [Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph. Microsoft.Graph.Auth tem uma dependência em Microsoft.Graph.Core.

Você pode usar a interface [do usuário Gerenciador de Pacotes no](/nuget/quickstart/install-and-use-a-package-in-visual-studio) Visual Studio ou o console Gerenciador de Pacotes para instalar os pacotes do Microsoft.Graph em seu projeto. Os comandos Gerenciador de Pacotes Console a seguir instalarão as bibliotecas Microsoft.Graph, Microsoft.Graph.Core e Microsoft.Graph.Auth. O Microsoft.Graph.Core é instalado como uma dependência do Microsoft.Graph.

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Instalar o Microsoft Graph Java SDK

O microsoft graph Java SDK está incluído nos seguintes pacotes:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade `beta` com a API fluente.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - A biblioteca principal para fazer chamadas para o Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Instalar o Microsoft Graph Java SDK via Gradle

Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do seu projeto:

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Instalar o microsoft graph Java SDK via Maven

Adicione os repositórios no `profiles` elemento em pom.xml:

```xml
<profiles>
    <profile>
        <repositories>
            <repository>
                <snapshots>
                    <enabled>false</enabled>
                </snapshots>
                <id>bintray-microsoftgraph-Maven</id>
                <name>bintray</name>
                <url>https://dl.bintray.com/microsoftgraph/Maven</url>
            </repository>
        </repositories>
    </profile>
</profiles>
```

Adicione a dependência no `dependencies` elemento em pom.xml:

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o SDK Javascript do Microsoft Graph

O SDK Javascript do Microsoft Graph está incluído nos seguintes pacotes:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- A biblioteca principal para fazer chamadas ao Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - Os tipos Typescript para as entidades do Microsoft Graph.

Você pode usar [npm](https://www.npmjs.com) para instalar o SDK Javascript do Microsoft Graph:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Instalar o SDK Do Microsoft Graph Objective-C

O SDK Do Microsoft Graph Objective-C dá suporte a plataformas iOS e macOS e pode ser instalado em seu projeto usando CocoaPods ou Cartago.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Instalar o SDK Objective-C do Microsoft Graph usando Cocoapods

Adicione a seguinte linha em seu arquivo de pod para incluir o SDK objective-C do Microsoft Graph e o SDK Auth objective-C do Microsoft Graph no seu projeto de xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Instalar o SDK Do Microsoft Graph Objective-C usando Cartago

Execute as etapas a seguir para instalar o SDK do Microsoft Graph Objective-C e o SDK do Microsoft Graph Objective-C Auth usando o gerenciador de pacotes [de](https://github.com/Carthage/Carthage) Cartago.

1. Crie um **Cartfile** que especifica o repositório e a marca de lançamento do GitHub do SDK Do Objective-C [para](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) o destino.

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Executar `carthage update` . Isso buscará dependências em uma pasta Cartago/Checkouts e criará a biblioteca MSGraphClientSDK.

1. Usando o Xcode, na  guia Configurações Gerais do destino do aplicativo, na seção **Estruturas Vinculadas e Bibliotecas,** arraste e solte a **MSGraphClientSDK.framework** e **MSGraphMSALAuthProvider.framework** da pasta Cartago/Complicação no disco.

1. Na guia **Fases** de Com build do destino do aplicativo, clique no ícone e **+** escolha Nova Fase de Script de **Executar.** Crie um script de executar no qual você especifique seu shell (ex: /bin/sh) e adicione o seguinte conteúdo ao script:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Adicione os caminhos às estruturas que você deseja usar em **Arquivos de Entrada**.

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>Instalar o SDK PHP do Microsoft Graph

O [SDK PHP](https://github.com/microsoftgraph/msgraph-sdk-php) do Microsoft Graph está disponível packagist.org [e](https://packagist.org/packages/microsoft/microsoft-graph) pode ser instalado das seguintes maneiras:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Instalar o SDK PHP do Microsoft Graph manualmente usando o compositor

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Instalar o SDK PHP do Microsoft Graph usando composer.json

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>Instalar o SDK do Microsoft PowerShell

Consulte [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Instalar o SDK ruby do Microsoft Graph

O [SDK ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) do Microsoft Graph está disponível no rubygems.org [e](https://rubygems.org/) pode ser instalado usando o seguinte comando:

```ruby
gem install microsoft_graph
```
