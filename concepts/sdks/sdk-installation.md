---
title: Instalar o Microsoft Graph SDK
description: Fornece instruções para instalar os SDKs C#, Java, Javascript, Objective-C, PHP e Ruby Microsoft Graph.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 770b1e72d418a3f0308651b8fdd93a5e2fb7e834
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848766"
---
# <a name="install-the-microsoft-graph-sdks"></a>Instalar os SDKs do Microsoft Graph

Os SDKs Graph Microsoft estão disponíveis para serem incluídos em seus projetos por meio de GitHub e gerenciadores de pacotes de plataforma populares. Este tópico descreve como você pode instalar o Microsoft Graph SDK em seu projeto.

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o SDK do Javascript do Microsoft Graph

O Microsoft Graph SDK javascript está incluído nos seguintes pacotes:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) – a biblioteca principal para fazer chamadas para o Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) – os tipos Typescript para as entidades do Microsoft Graph.

Você pode usar [o npm](https://www.npmjs.com) para instalar o SDK do Microsoft Graph Javascript:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Instalar o SDK do Microsoft Graph Objective-C

O SDK do Microsoft Graph Objective-C dá suporte a plataformas iOS e macOS e pode ser instalado em seu projeto usando CocoaPods ou Carthage.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Instalar o SDK do Microsoft Graph Objective-C usando Cocoapods

Adicione a seguinte linha em seu podfile para incluir o SDK do Objective-C Microsoft Graph e o SDK de Autenticação Objective-C do Microsoft Graph em seu projeto xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Instalar o SDK do Microsoft Graph Objective-C usando o Carthage

Execute as etapas a seguir para instalar o SDK do Microsoft Graph Objective-C e o SDK de Autenticação Objective-C do Microsoft Graph usando o gerenciador de pacotes [do Carthage](https://github.com/Carthage/Carthage).

1. Crie um **Cartfile** que especifica o SDK do Objective-C GitHub e a marca [de versão](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) para o destino.

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Execute `carthage update`. Isso buscará dependências em uma pasta Carthage/Checkouts e criará a biblioteca MSGraphClientSDK.

1. Usando o Xcode, na guia Configurações Gerais  do destino do aplicativo, na seção **Estruturas Vinculadas e Bibliotecas**, arraste e solte o **MSGraphClientSDK.framework** e **o MSGraphMSALAuthProvider.framework** da pasta Carthage/Build no disco.

1. Na guia Configurações de **Fases de Build** do destino do aplicativo, clique **+** no ícone e escolha **Nova Fase de Script de Execução**. Crie um script de execução no qual você especifique seu shell (por exemplo: /bin/sh) e adicione o seguinte conteúdo ao script:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Adicione os caminhos às estruturas que você deseja usar em Arquivos **de Entrada**.

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
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

## <a name="install-the-microsoft-powershell-sdk"></a>Instalar o SDK do Microsoft PowerShell

Consulte [Instalar o SDK do PowerShell do Microsoft Graph](/powershell/microsoftgraph/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Instalar o Microsoft Graph Ruby SDK

O [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) está disponível no [rubygems.org](https://rubygems.org/) e pode ser instalado usando o seguinte comando:

```ruby
gem install microsoft_graph
```
