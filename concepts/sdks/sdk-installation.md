---
title: Instalar o Microsoft Graph SDK
description: Fornece instruções para instalar os C#, Java, Javascript, Objective-C, PHP e Ruby Microsoft Graph SDKs.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 1133e8f4cd1d0690c5a8ff6ef818c29294b3d2ee
ms.sourcegitcommit: 1ae0079021dfcbcc910dcdc74440d367ec4af7d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63460123"
---
# <a name="install-the-microsoft-graph-sdks"></a>Instalar os SDKs Graph Microsoft

Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio GitHub e gerentes de pacote de plataforma populares. Este tópico descreve como você pode instalar o Microsoft Graph SDK em seu projeto.

## <a name="install-the-microsoft-graph-net-sdk"></a>Instalar o SDK do Microsoft Graph .NET

O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente. Microsoft. Graph tem uma dependência da Microsoft. Graph. Core.
- [Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o `beta` ponto de extremidade com a API fluente. Microsoft. Graph. Beta tem uma dependência da Microsoft. Graph. Core.
- [Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - A biblioteca principal para fazer chamadas para o Microsoft Graph.

Você pode usar a interface [do usuário Gerenciador de Pacotes no Visual Studio ou o console Gerenciador de Pacotes](/nuget/quickstart/install-and-use-a-package-in-visual-studio) para instalar os pacotes microsoft.Graph em seu projeto. Os comandos Gerenciador de Pacotes Console a seguir instalarão o Microsoft.Graph e o Microsoft.Graph. Bibliotecas principais. Microsoft. Graph. Core é instalado como uma dependência da Microsoft. Graph.

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>Instalar o Microsoft Graph Go SDK (visualização)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

O Microsoft Graph Go SDK está incluído nos seguintes pacotes:

- [Microsoft Graph SDK para Go](https://github.com/microsoftgraph/msgraph-sdk-go) - `v1.0` Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade com a API fluente.
- [Microsoft Graph Beta SDK para Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go) - `beta` Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade com a API fluente.
- [Microsoft Graph SDK Principal para Ir](https://github.com/microsoftgraph/msgraph-sdk-go-core) - A biblioteca principal para fazer chamadas para o Microsoft Graph.

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota/authentication/go/azure
```

## <a name="install-the-microsoft-graph-java-sdk"></a>Instalar o Microsoft Graph Java SDK

O Microsoft Graph Java SDK está incluído nos seguintes pacotes:

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente.
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o `beta` ponto de extremidade com a API fluente.
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - A biblioteca principal para fazer chamadas para o Microsoft Graph.
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o Microsoft Graph SDK.

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>Instalar o Microsoft Graph Java SDK via Gradle

Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do seu projeto:

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

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>Instalar o Microsoft Graph Java SDK via Maven

Adicione a dependência no elemento em `dependencies` pom.xml:

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a>Instalar o Microsoft Graph Javascript SDK

O Microsoft Graph Javascript SDK está incluído nos seguintes pacotes:

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- A biblioteca principal para fazer chamadas para o Microsoft Graph.
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - Os tipos Typescript para as entidades Graph Microsoft.

Você pode usar [npm](https://www.npmjs.com) para instalar o Microsoft Graph Javascript SDK:

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>Instalar o SDK do Microsoft Graph Objective-C

O SDK do Microsoft Graph Objective-C dá suporte a plataformas iOS e macOS e pode ser instalado em seu projeto usando CocoaPods ou Cartago.

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>Instalar o SDK do Microsoft Graph Objective-C usando Cocoapods

Adicione a seguinte linha em seu arquivo de pod para incluir o SDK objective-C microsoft Graph e o SDK do Microsoft Graph Objective-C Auth em seu projeto de xcode:

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>Instalar o SDK do Microsoft Graph Objective-C usando Cartago

Execute as etapas a seguir para instalar o SDK do Microsoft Graph Objective-C e o SDK do Microsoft Graph Objective-C Auth usando o gerenciador de [](https://github.com/Carthage/Carthage) pacotes de carta.

1. Crie um **Cartfile** que especifica o SDK Objective-C GitHub repositório e a [marca de versão](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) para o destino.

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. Execute `carthage update`. Isso buscará dependências em uma pasta Cartago/Checkouts e criará a biblioteca MSGraphClientSDK.

1. Usando o Xcode, na guia Configurações Gerais  do destino do aplicativo, na seção **Estruturas Vinculadas e Bibliotecas**, arraste e solte a **MSGraphClientSDK.framework** e **MSGraphMSALAuthProvider.framework** da pasta Cartago/Complicação no disco.

1. Na guia **Fases** de Com build do destino do aplicativo, clique **+** no ícone e escolha **Nova Fase de Script de Executar**. Crie um script de executar no qual você especifique seu shell (ex: /bin/sh) e adicione o seguinte conteúdo ao script:

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. Adicione os caminhos às estruturas que você deseja usar em **Arquivos de Entrada**.

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>Instalar o Microsoft Graph PHP SDK

O [Microsoft Graph SDK PHP](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível no [packagist.org e pode](https://packagist.org/packages/microsoft/microsoft-graph) ser instalado das seguintes maneiras:

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>Instalar o Microsoft Graph PHP SDK manualmente usando o compositor

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>Instalar o Microsoft Graph PHP SDK usando composer.json

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>Instalar o SDK do Microsoft PowerShell

Consulte [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).

## <a name="install-the-microsoft-graph-ruby-sdk"></a>Instalar o Microsoft Graph Ruby SDK

O [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) está disponível no rubygems.org e pode [](https://rubygems.org/) ser instalado usando o seguinte comando:

```ruby
gem install microsoft_graph
```
