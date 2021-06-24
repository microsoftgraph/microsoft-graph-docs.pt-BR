---
title: Instalar o Microsoft Graph PowerShell SDK
description: Fornece instruções para instalar o Microsoft Graph PowerShell SDK.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 58e967d7acedbbfe4f8c3781a7ec796e697a44c8
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107673"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="94bf4-103">Instalar o Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="94bf4-103">Install the Microsoft Graph PowerShell SDK</span></span>

> [!NOTE]
> <span data-ttu-id="94bf4-104">A instalação do módulo principal do SDK instalará todos os 38 sub módulos.</span><span class="sxs-lookup"><span data-stu-id="94bf4-104">Installing the main module of the SDK will install all 38 sub modules.</span></span> <span data-ttu-id="94bf4-105">Considere apenas instalar os módulos necessários, incluindo `Microsoft.Graph.Authentication` .</span><span class="sxs-lookup"><span data-stu-id="94bf4-105">Consider only installing the neccessary modules, including `Microsoft.Graph.Authentication`.</span></span>

<span data-ttu-id="94bf4-106">O SDK do Microsoft Graph PowerShell é publicado na [Galeria do PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph)</span><span class="sxs-lookup"><span data-stu-id="94bf4-106">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="94bf4-107">Você pode instalar o SDK no PowerShell Core ou Windows PowerShell usando o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="94bf4-107">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

<span data-ttu-id="94bf4-108">Opcionalmente, você pode alterar o escopo da instalação usando o `-Scope` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="94bf4-108">Optionally, you can change the scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="94bf4-109">Isso requer permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="94bf4-109">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="94bf4-110">Instalar o SDK em uma versão do PowerShell não o instala para a outra.</span><span class="sxs-lookup"><span data-stu-id="94bf4-110">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="94bf4-111">Certifique-se de executar o comando de instalação dentro da versão do PowerShell em que você pretende usá-lo.</span><span class="sxs-lookup"><span data-stu-id="94bf4-111">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="94bf4-112">Verificar a instalação</span><span class="sxs-lookup"><span data-stu-id="94bf4-112">Verify installation</span></span>

<span data-ttu-id="94bf4-113">Após a conclusão da instalação, você pode verificar a versão instalada com o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="94bf4-113">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="94bf4-114">A versão na saída deve corresponder à versão mais recente publicada na Galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="94bf4-114">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="94bf4-115">Agora você está pronto para usar o SDK.</span><span class="sxs-lookup"><span data-stu-id="94bf4-115">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="94bf4-116">Começar com o Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="94bf4-116">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="94bf4-117">Atualizando o SDK</span><span class="sxs-lookup"><span data-stu-id="94bf4-117">Updating the SDK</span></span>

<span data-ttu-id="94bf4-118">Você pode atualizar o SDK e todas as suas dependências usando o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="94bf4-118">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="94bf4-119">Desinstalar o SDK</span><span class="sxs-lookup"><span data-stu-id="94bf4-119">Uninstalling the SDK</span></span>

<span data-ttu-id="94bf4-120">Primeiro, use o seguinte comando para desinstalar o módulo principal.</span><span class="sxs-lookup"><span data-stu-id="94bf4-120">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="94bf4-121">Em seguida, remova todos os módulos de dependência executando os seguintes comandos.</span><span class="sxs-lookup"><span data-stu-id="94bf4-121">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="94bf4-122">Faça comentários</span><span class="sxs-lookup"><span data-stu-id="94bf4-122">Provide feedback</span></span>

<span data-ttu-id="94bf4-123">Comentários de boas-vindas!</span><span class="sxs-lookup"><span data-stu-id="94bf4-123">We welcome feedback!</span></span> <span data-ttu-id="94bf4-124">Forneça comentários ou informe quaisquer problemas no [repositório GitHub SDK.](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)</span><span class="sxs-lookup"><span data-stu-id="94bf4-124">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>
