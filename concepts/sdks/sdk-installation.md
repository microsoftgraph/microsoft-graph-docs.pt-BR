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
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="f807b-103">Instalar os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f807b-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="f807b-104">Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio do GitHub e gerentes de pacotes de plataforma populares.</span><span class="sxs-lookup"><span data-stu-id="f807b-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="f807b-105">Este tópico descreve como você pode instalar o SDK do Microsoft Graph em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="f807b-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="f807b-106">Instalar o SDK do Microsoft Graph .NET</span><span class="sxs-lookup"><span data-stu-id="f807b-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="f807b-107">O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:</span><span class="sxs-lookup"><span data-stu-id="f807b-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="f807b-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="f807b-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="f807b-109">O Microsoft.Graph tem uma dependência do Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="f807b-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="f807b-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade `beta` com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="f807b-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="f807b-111">O Microsoft.Graph.Beta tem uma dependência do Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="f807b-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="f807b-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - A biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f807b-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="f807b-114">Microsoft.Graph.Auth tem uma dependência em Microsoft.Graph.Core.</span><span class="sxs-lookup"><span data-stu-id="f807b-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="f807b-115">Você pode usar a interface [do usuário Gerenciador de Pacotes no](/nuget/quickstart/install-and-use-a-package-in-visual-studio) Visual Studio ou o console Gerenciador de Pacotes para instalar os pacotes do Microsoft.Graph em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="f807b-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="f807b-116">Os comandos Gerenciador de Pacotes Console a seguir instalarão as bibliotecas Microsoft.Graph, Microsoft.Graph.Core e Microsoft.Graph.Auth.</span><span class="sxs-lookup"><span data-stu-id="f807b-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="f807b-117">O Microsoft.Graph.Core é instalado como uma dependência do Microsoft.Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="f807b-118">Instalar o Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="f807b-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="f807b-119">O microsoft graph Java SDK está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="f807b-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="f807b-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto `v1.0` de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="f807b-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="f807b-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contém os modelos e os construtores de solicitação para acessar o ponto de extremidade `beta` com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="f807b-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="f807b-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - A biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f807b-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Fornece um wrapper baseado em cenário de autenticação da Biblioteca de Autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="f807b-124">Instalar o Microsoft Graph Java SDK via Gradle</span><span class="sxs-lookup"><span data-stu-id="f807b-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="f807b-125">Adicione o repositório e uma dependência de compilação do microsoft-graph ao build.gradle do seu projeto:</span><span class="sxs-lookup"><span data-stu-id="f807b-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="f807b-126">Instalar o microsoft graph Java SDK via Maven</span><span class="sxs-lookup"><span data-stu-id="f807b-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="f807b-127">Adicione os repositórios no `profiles` elemento em pom.xml:</span><span class="sxs-lookup"><span data-stu-id="f807b-127">Add the repositories in the `profiles` element in pom.xml:</span></span>

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

<span data-ttu-id="f807b-128">Adicione a dependência no `dependencies` elemento em pom.xml:</span><span class="sxs-lookup"><span data-stu-id="f807b-128">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="f807b-129">Instalar o SDK Javascript do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f807b-129">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="f807b-130">O SDK Javascript do Microsoft Graph está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="f807b-130">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="f807b-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- A biblioteca principal para fazer chamadas ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="f807b-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - Os tipos Typescript para as entidades do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f807b-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="f807b-133">Você pode usar [npm](https://www.npmjs.com) para instalar o SDK Javascript do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="f807b-133">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="f807b-134">Instalar o SDK Do Microsoft Graph Objective-C</span><span class="sxs-lookup"><span data-stu-id="f807b-134">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="f807b-135">O SDK Do Microsoft Graph Objective-C dá suporte a plataformas iOS e macOS e pode ser instalado em seu projeto usando CocoaPods ou Cartago.</span><span class="sxs-lookup"><span data-stu-id="f807b-135">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="f807b-136">Instalar o SDK Objective-C do Microsoft Graph usando Cocoapods</span><span class="sxs-lookup"><span data-stu-id="f807b-136">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="f807b-137">Adicione a seguinte linha em seu arquivo de pod para incluir o SDK objective-C do Microsoft Graph e o SDK Auth objective-C do Microsoft Graph no seu projeto de xcode:</span><span class="sxs-lookup"><span data-stu-id="f807b-137">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="f807b-138">Instalar o SDK Do Microsoft Graph Objective-C usando Cartago</span><span class="sxs-lookup"><span data-stu-id="f807b-138">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="f807b-139">Execute as etapas a seguir para instalar o SDK do Microsoft Graph Objective-C e o SDK do Microsoft Graph Objective-C Auth usando o gerenciador de pacotes [de](https://github.com/Carthage/Carthage) Cartago.</span><span class="sxs-lookup"><span data-stu-id="f807b-139">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="f807b-140">Crie um **Cartfile** que especifica o repositório e a marca de lançamento do GitHub do SDK Do Objective-C [para](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) o destino.</span><span class="sxs-lookup"><span data-stu-id="f807b-140">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="f807b-141">Executar `carthage update` .</span><span class="sxs-lookup"><span data-stu-id="f807b-141">Run `carthage update`.</span></span> <span data-ttu-id="f807b-142">Isso buscará dependências em uma pasta Cartago/Checkouts e criará a biblioteca MSGraphClientSDK.</span><span class="sxs-lookup"><span data-stu-id="f807b-142">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="f807b-143">Usando o Xcode, na  guia Configurações Gerais do destino do aplicativo, na seção **Estruturas Vinculadas e Bibliotecas,** arraste e solte a **MSGraphClientSDK.framework** e **MSGraphMSALAuthProvider.framework** da pasta Cartago/Complicação no disco.</span><span class="sxs-lookup"><span data-stu-id="f807b-143">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="f807b-144">Na guia **Fases** de Com build do destino do aplicativo, clique no ícone e **+** escolha Nova Fase de Script de **Executar.**</span><span class="sxs-lookup"><span data-stu-id="f807b-144">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="f807b-145">Crie um script de executar no qual você especifique seu shell (ex: /bin/sh) e adicione o seguinte conteúdo ao script:</span><span class="sxs-lookup"><span data-stu-id="f807b-145">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="f807b-146">Adicione os caminhos às estruturas que você deseja usar em **Arquivos de Entrada**.</span><span class="sxs-lookup"><span data-stu-id="f807b-146">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="f807b-147">Instalar o SDK PHP do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f807b-147">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="f807b-148">O [SDK PHP](https://github.com/microsoftgraph/msgraph-sdk-php) do Microsoft Graph está disponível packagist.org [e](https://packagist.org/packages/microsoft/microsoft-graph) pode ser instalado das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="f807b-148">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="f807b-149">Instalar o SDK PHP do Microsoft Graph manualmente usando o compositor</span><span class="sxs-lookup"><span data-stu-id="f807b-149">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="f807b-150">Instalar o SDK PHP do Microsoft Graph usando composer.json</span><span class="sxs-lookup"><span data-stu-id="f807b-150">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="f807b-151">Instalar o SDK do Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="f807b-151">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="f807b-152">Consulte [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span><span class="sxs-lookup"><span data-stu-id="f807b-152">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="f807b-153">Instalar o SDK ruby do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f807b-153">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="f807b-154">O [SDK ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) do Microsoft Graph está disponível no rubygems.org [e](https://rubygems.org/) pode ser instalado usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="f807b-154">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
