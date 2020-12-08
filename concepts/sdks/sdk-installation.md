---
title: Instalar o SDK do Microsoft Graph
description: Fornece instruções para a instalação dos SDKs C#, Java, JavaScript, Objective-C, PHP e Ruby do Microsoft Graph.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7f96266c1ff774f52e559737fe67f032f1e54fdc
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580953"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="80fc5-103">Instalar os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="80fc5-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="80fc5-104">Os SDKs do Microsoft Graph estão disponíveis para serem incluídos em seus projetos por meio do GitHub e gerentes de pacotes de plataforma populares.</span><span class="sxs-lookup"><span data-stu-id="80fc5-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="80fc5-105">Este tópico descreve como você pode instalar o SDK do Microsoft Graph em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="80fc5-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="80fc5-106">Instalar o SDK do Microsoft Graph .NET</span><span class="sxs-lookup"><span data-stu-id="80fc5-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="80fc5-107">O SDK do Microsoft Graph .NET está incluído nos seguintes pacotes NuGet:</span><span class="sxs-lookup"><span data-stu-id="80fc5-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="80fc5-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -contém os modelos e criadores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="80fc5-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="80fc5-109">O Microsoft. Graph tem uma dependência em Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="80fc5-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="80fc5-110">[Microsoft. Graph. beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -contém os modelos e criadores de solicitação para acessar o `beta` ponto de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="80fc5-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="80fc5-111">Microsoft. Graph. beta tem uma dependência em Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="80fc5-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="80fc5-112">[Microsoft. Graph. Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -a biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="80fc5-113">[Microsoft. Graph. auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) : fornece um wrapper baseado em cenário de autenticação da biblioteca de autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="80fc5-114">Microsoft. Graph. auth tem uma dependência em Microsoft. Graph. Core.</span><span class="sxs-lookup"><span data-stu-id="80fc5-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="80fc5-115">Você pode usar a [interface do usuário do Gerenciador de pacotes no Visual Studio ou no console do Gerenciador de pacotes](/nuget/quickstart/install-and-use-a-package-in-visual-studio) para instalar os pacotes do Microsoft. Graph em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="80fc5-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="80fc5-116">Os seguintes comandos do console do Gerenciador de pacotes instalarão as bibliotecas Microsoft. Graph, Microsoft. Graph. Core e Microsoft. Graph. auth.</span><span class="sxs-lookup"><span data-stu-id="80fc5-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="80fc5-117">O Microsoft. Graph. Core é instalado como uma dependência de Microsoft. Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="80fc5-118">Instalar o SDK do Microsoft Graph Java</span><span class="sxs-lookup"><span data-stu-id="80fc5-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="80fc5-119">O SDK do Microsoft Graph Java está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="80fc5-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="80fc5-120">[Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) -contém os modelos e criadores de solicitação para acessar o `v1.0` ponto de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="80fc5-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="80fc5-121">[Microsoft-Graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) -contém os modelos e criadores de solicitação para acessar o `beta` ponto de extremidade com a API fluente.</span><span class="sxs-lookup"><span data-stu-id="80fc5-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="80fc5-122">[Microsoft-Graph-Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -a biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="80fc5-123">[Microsoft-Graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -fornece um wrapper baseado em cenário de autenticação da biblioteca de autenticação da Microsoft (MSAL) para uso com o SDK do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="80fc5-124">Instalar o SDK do Microsoft Graph Java via gradle</span><span class="sxs-lookup"><span data-stu-id="80fc5-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="80fc5-125">Adicione o repositório e uma dependência de compilação do Microsoft-Graph à compilação do seu projeto. gradle:</span><span class="sxs-lookup"><span data-stu-id="80fc5-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
    jcenter{
        url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
    }
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:2.+'
    implementation 'com.microsoft.graph:microsoft-graph-auth:0.3.0'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="80fc5-126">Instalar o SDK do Microsoft Graph Java via Maven</span><span class="sxs-lookup"><span data-stu-id="80fc5-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="80fc5-127">Adicione os repositórios no `profiles` elemento no pom.xml:</span><span class="sxs-lookup"><span data-stu-id="80fc5-127">Add the repositories in the `profiles` element in pom.xml:</span></span>

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
    <profile>
       <id>allow-snapshots</id>
          <activation><activeByDefault>true</activeByDefault></activation>
       <repositories>
         <repository>
           <id>snapshots-repo</id>
           <url>https://oss.sonatype.org/content/repositories/snapshots</url>
           <releases><enabled>false</enabled></releases>
           <snapshots><enabled>true</enabled></snapshots>
         </repository>
       </repositories>
     </profile>
</profiles>
```

<span data-ttu-id="80fc5-128">Adicione a dependência no `dependencies` elemento no pom.xml:</span><span class="sxs-lookup"><span data-stu-id="80fc5-128">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[2.0,)</version>
</dependency>
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph-auth</artifactId>
    <version>0.3.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="80fc5-129">Instalar o SDK do JavaScript do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="80fc5-129">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="80fc5-130">O SDK do JavaScript do Microsoft Graph está incluído nos seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="80fc5-130">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="80fc5-131">@microsoft/Microsoft-Graph-Client ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))-a biblioteca principal para fazer chamadas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="80fc5-132">@microsoft/Microsoft-Graph-Types ([NPM](https://www.npmjs.com/package/@microsoft/microsoft-graph-types))-os tipos de typescript para entidades do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="80fc5-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="80fc5-133">Você pode usar o [NPM](https://www.npmjs.com) para instalar o SDK do JavaScript do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="80fc5-133">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="80fc5-134">Instalar o SDK do Microsoft Graph objetivo-C</span><span class="sxs-lookup"><span data-stu-id="80fc5-134">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="80fc5-135">O SDK do Microsoft Graph objetivo-C suporta as plataformas iOS e macOS e pode ser instalado em seu projeto usando o CocoaPods ou o Carthage.</span><span class="sxs-lookup"><span data-stu-id="80fc5-135">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="80fc5-136">Instale o SDK do Microsoft Graph objetivo-C usando Cocoapods</span><span class="sxs-lookup"><span data-stu-id="80fc5-136">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="80fc5-137">Adicione a seguinte linha no seu podfile para incluir o SDK do Microsoft Graph objetivo e o SDK do Microsoft Graph objetivo-C de autenticação no seu projeto do Xcode:</span><span class="sxs-lookup"><span data-stu-id="80fc5-137">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="80fc5-138">Instale o SDK do Microsoft Graph objetivo-C usando Carthage</span><span class="sxs-lookup"><span data-stu-id="80fc5-138">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="80fc5-139">Execute as seguintes etapas para instalar o Microsoft Graph objector-C SDK e o Microsoft Graph Objective SDK-C auth using the [Carthage](https://github.com/Carthage/Carthage) Package Manager.</span><span class="sxs-lookup"><span data-stu-id="80fc5-139">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="80fc5-140">Crie um **cartfile** que especifica o repositório e a [marca de versão](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) do SDK do</span><span class="sxs-lookup"><span data-stu-id="80fc5-140">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="80fc5-141">Executar `carthage update` .</span><span class="sxs-lookup"><span data-stu-id="80fc5-141">Run `carthage update`.</span></span> <span data-ttu-id="80fc5-142">Isso irá buscar dependências em uma pasta Carthage/checkouts e, em seguida, cria a biblioteca MSGraphClientSDK.</span><span class="sxs-lookup"><span data-stu-id="80fc5-142">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="80fc5-143">Usando o Xcode, na guia configurações **gerais** da sua meta de aplicativo, na seção **estruturas e bibliotecas vinculadas** , arraste e solte o **MSGraphClientSDK. Framework** e o **MSGraphMSALAuthProvider. Framework** da pasta Carthage/Build no disco.</span><span class="sxs-lookup"><span data-stu-id="80fc5-143">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="80fc5-144">Na guia Configurações de **fases de compilação** do seu destino de aplicativo, clique no **+** ícone e escolha **nova fase de script de execução**.</span><span class="sxs-lookup"><span data-stu-id="80fc5-144">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="80fc5-145">Crie um script de execução em que você especifique seu shell (ex:/bin/sh) e adicione o seguinte conteúdo ao script:</span><span class="sxs-lookup"><span data-stu-id="80fc5-145">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="80fc5-146">Adicione os caminhos para os frameworks que você deseja usar em **arquivos de entrada**.</span><span class="sxs-lookup"><span data-stu-id="80fc5-146">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="80fc5-147">Instalar o SDK do Microsoft Graph PHP</span><span class="sxs-lookup"><span data-stu-id="80fc5-147">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="80fc5-148">O [SDK do Microsoft Graph php](https://github.com/microsoftgraph/msgraph-sdk-php) está disponível no [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) e pode ser instalado das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="80fc5-148">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="80fc5-149">Instalar o SDK do Microsoft Graph PHP manualmente usando o Composer</span><span class="sxs-lookup"><span data-stu-id="80fc5-149">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="80fc5-150">Instale o SDK do Microsoft Graph PHP usando composer.jsno</span><span class="sxs-lookup"><span data-stu-id="80fc5-150">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="80fc5-151">Instalar o SDK do Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="80fc5-151">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="80fc5-152">Confira [instalar o SDK do Microsoft Graph PowerShell](../powershell/installation.md).</span><span class="sxs-lookup"><span data-stu-id="80fc5-152">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="80fc5-153">Instalar o SDK do Microsoft Graph Ruby</span><span class="sxs-lookup"><span data-stu-id="80fc5-153">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="80fc5-154">O [SDK do Microsoft Graph Ruby](https://github.com/microsoftgraph/msgraph-sdk-ruby) está disponível no [RubyGems.org](https://rubygems.org/) e pode ser instalado usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="80fc5-154">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
