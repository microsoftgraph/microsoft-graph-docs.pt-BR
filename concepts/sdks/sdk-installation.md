---
title: Instalar o Microsoft Graph SDK
description: Fornece instruções para instalar os C#, Java, Javascript, Objective-C, PHP e Ruby Microsoft Graph SDKs.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 96f2df7f928ba516d4cd0278bc560983cd355893
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475525"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="1540b-103">Instalar os SDKs Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="1540b-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="1540b-104">Os SDKs Graph Microsoft estão disponíveis para serem incluídos em seus projetos por meio de GitHub e gerentes de pacote de plataforma populares.</span><span class="sxs-lookup"><span data-stu-id="1540b-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="1540b-105">Este tópico descreve como você pode instalar o Microsoft Graph SDK em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="1540b-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="1540b-106">Instalar o SDK do Microsoft Graph .NET</span><span class="sxs-lookup"><span data-stu-id="1540b-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="1540b-107">O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:</span><span class="sxs-lookup"><span data-stu-id="1540b-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="1540b-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="1540b-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="1540b-109">Microsoft. Graph tem uma dependência da Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="1540b-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="1540b-110">[Microsoft. Graph. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto `beta` de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="1540b-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="1540b-111">Microsoft. Graph. Beta tem uma dependência da Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="1540b-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="1540b-112">[Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - A biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1540b-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="1540b-113">[Microsoft. Graph. Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o Microsoft Graph SDK.</span><span class="sxs-lookup"><span data-stu-id="1540b-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="1540b-114">Microsoft. Graph. A Auth tem uma dependência da Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="1540b-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="1540b-115">Você pode usar a interface Gerenciador de Pacotes interface do usuário no Visual Studio ou o [console Gerenciador de Pacotes para](/nuget/quickstart/install-and-use-a-package-in-visual-studio) instalar a Microsoft. Graph pacotes em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="1540b-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="1540b-116">Os comandos Gerenciador de Pacotes Console a seguir instalarão a Microsoft. Graph, Microsoft. Graph. Core e Microsoft. Graph. Bibliotecas de auth.</span><span class="sxs-lookup"><span data-stu-id="1540b-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="1540b-117">Microsoft. Graph. Core é instalado como uma dependência da Microsoft. Graph.</span><span class="sxs-lookup"><span data-stu-id="1540b-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="1540b-118">Instalar o Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="1540b-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="1540b-119">O Microsoft Graph Java SDK está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="1540b-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="1540b-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="1540b-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="1540b-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade `beta` com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="1540b-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="1540b-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - a biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1540b-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="1540b-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o Microsoft Graph SDK.</span><span class="sxs-lookup"><span data-stu-id="1540b-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="1540b-124">Instalar o Microsoft Graph Java SDK via Gradle</span><span class="sxs-lookup"><span data-stu-id="1540b-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="1540b-125">Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do seu projeto:</span><span class="sxs-lookup"><span data-stu-id="1540b-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    mavenCentral()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
    // Include Azure identity for authentication
    implementation 'com.azure:azure-identity:1.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="1540b-126">Instalar o Microsoft Graph Java SDK via Maven</span><span class="sxs-lookup"><span data-stu-id="1540b-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="1540b-127">Adicione a dependência no `dependencies` elemento em pom.xml:</span><span class="sxs-lookup"><span data-stu-id="1540b-127">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.3,)</version>
</dependency>
<dependency>
    <groupId>com.azure</groupId>
    <artifactId>azure-identity</artifactId>
    <version>[1.2,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="1540b-128">Instalar o Microsoft Graph Javascript SDK</span><span class="sxs-lookup"><span data-stu-id="1540b-128">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="1540b-129">O Microsoft Graph Javascript SDK está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="1540b-129">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="1540b-130">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- A biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1540b-130">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="1540b-131">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - Os tipos Typescript para as entidades Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1540b-131">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="1540b-132">Você pode usar [npm](https://www.npmjs.com) para instalar o Microsoft Graph Javascript SDK:</span><span class="sxs-lookup"><span data-stu-id="1540b-132">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="1540b-133">Instalar o SDK do Microsoft Graph Objective-C</span><span class="sxs-lookup"><span data-stu-id="1540b-133">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="1540b-134">O Microsoft Graph Objective-C SDK dá suporte a plataformas iOS e macOS e pode ser instalado em seu projeto usando CocoaPods ou Cartago.</span><span class="sxs-lookup"><span data-stu-id="1540b-134">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="1540b-135">Instalar o SDK do Microsoft Graph Objective-C usando Cocoapods</span><span class="sxs-lookup"><span data-stu-id="1540b-135">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="1540b-136">Adicione a seguinte linha em seu arquivo de pod para incluir o SDK objective-C microsoft Graph e o SDK do Microsoft Graph Objective-C Auth em seu projeto de xcode:</span><span class="sxs-lookup"><span data-stu-id="1540b-136">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="1540b-137">Instalar o SDK do Microsoft Graph Objective-C usando Cartago</span><span class="sxs-lookup"><span data-stu-id="1540b-137">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="1540b-138">Execute as etapas a seguir para instalar o SDK do Microsoft Graph Objective-C e o [](https://github.com/Carthage/Carthage) SDK do Microsoft Graph Objective-C Auth usando o gerenciador de pacotes de Cartago.</span><span class="sxs-lookup"><span data-stu-id="1540b-138">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="1540b-139">Crie um **Cartfile** que especifica o SDK Objective-C GitHub repositório e a [marca de versão](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) para o destino.</span><span class="sxs-lookup"><span data-stu-id="1540b-139">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="1540b-140">Executar `carthage update` .</span><span class="sxs-lookup"><span data-stu-id="1540b-140">Run `carthage update`.</span></span> <span data-ttu-id="1540b-141">Isso buscará dependências em uma pasta Cartago/Checkouts e criará a biblioteca MSGraphClientSDK.</span><span class="sxs-lookup"><span data-stu-id="1540b-141">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="1540b-142">Usando o Xcode, na  guia Configurações Gerais do destino do aplicativo, na seção **Estruturas Vinculadas e Bibliotecas,** arraste e solte a **MSGraphClientSDK.framework** e **MSGraphMSALAuthProvider.framework** da pasta Cartago/Complicação no disco.</span><span class="sxs-lookup"><span data-stu-id="1540b-142">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="1540b-143">Na guia **Fases** de Com build do destino do aplicativo, clique no ícone e **+** escolha Nova Fase de Script de **Executar.**</span><span class="sxs-lookup"><span data-stu-id="1540b-143">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="1540b-144">Crie um script de executar no qual você especifique seu shell (ex: /bin/sh) e adicione o seguinte conteúdo ao script:</span><span class="sxs-lookup"><span data-stu-id="1540b-144">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="1540b-145">Adicione os caminhos às estruturas que você deseja usar em **Arquivos de Entrada**.</span><span class="sxs-lookup"><span data-stu-id="1540b-145">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="1540b-146">Instalar o Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="1540b-146">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="1540b-147">O [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível no packagist.org e pode ser instalado das seguintes maneiras: [](https://packagist.org/packages/microsoft/microsoft-graph)</span><span class="sxs-lookup"><span data-stu-id="1540b-147">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="1540b-148">Instalar o Microsoft Graph PHP SDK manualmente usando o compositor</span><span class="sxs-lookup"><span data-stu-id="1540b-148">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="1540b-149">Instalar o Microsoft Graph PHP SDK usando composer.json</span><span class="sxs-lookup"><span data-stu-id="1540b-149">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="1540b-150">Instalar o SDK do Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="1540b-150">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="1540b-151">Consulte [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span><span class="sxs-lookup"><span data-stu-id="1540b-151">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="1540b-152">Instalar o Microsoft Graph Ruby SDK</span><span class="sxs-lookup"><span data-stu-id="1540b-152">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="1540b-153">O [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) está [](https://rubygems.org/) disponível no rubygems.org e pode ser instalado usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="1540b-153">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
