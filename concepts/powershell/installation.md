---
title: Instalar o SDK do Microsoft Graph PowerShell
description: Fornece instruções para instalar o SDK do Microsoft Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 245cf03c8edf04a43c563bd19832eb0a35cf7cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193645"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="a07da-103">Instalar o SDK do Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="a07da-103">Install the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="a07da-104">O SDK do Microsoft Graph PowerShell é publicado na [Galeria do PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph).</span><span class="sxs-lookup"><span data-stu-id="a07da-104">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="a07da-105">Você pode instalar o SDK no PowerShell core ou no Windows PowerShell usando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="a07da-105">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph
```

<span data-ttu-id="a07da-106">Opcionalmente, você pode alterar o escopo padrão da instalação usando o `-Scope` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a07da-106">Optionally, you can change the default scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="a07da-107">Isso exige permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a07da-107">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="a07da-108">A instalação do SDK em uma versão do PowerShell não o instala para o outro.</span><span class="sxs-lookup"><span data-stu-id="a07da-108">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="a07da-109">Certifique-se de executar o comando de instalação dentro da versão do PowerShell em que você pretende usá-lo.</span><span class="sxs-lookup"><span data-stu-id="a07da-109">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="a07da-110">Verificar a instalação</span><span class="sxs-lookup"><span data-stu-id="a07da-110">Verify installation</span></span>

<span data-ttu-id="a07da-111">Após a conclusão da instalação, você pode verificar a versão instalada com o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="a07da-111">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="a07da-112">A versão na saída deve corresponder à versão mais recente publicada na galeria do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a07da-112">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="a07da-113">Agora você está pronto para usar o SDK.</span><span class="sxs-lookup"><span data-stu-id="a07da-113">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a07da-114">Introdução ao SDK do Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="a07da-114">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="a07da-115">Atualizando o SDK</span><span class="sxs-lookup"><span data-stu-id="a07da-115">Updating the SDK</span></span>

<span data-ttu-id="a07da-116">Você pode atualizar o SDK e todas as suas dependências usando o comando a seguir.</span><span class="sxs-lookup"><span data-stu-id="a07da-116">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="a07da-117">Desinstalando o SDK</span><span class="sxs-lookup"><span data-stu-id="a07da-117">Uninstalling the SDK</span></span>

<span data-ttu-id="a07da-118">Primeiro, use o comando a seguir para desinstalar o módulo principal.</span><span class="sxs-lookup"><span data-stu-id="a07da-118">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="a07da-119">Em seguida, remova todos os módulos de dependência executando os seguintes comandos.</span><span class="sxs-lookup"><span data-stu-id="a07da-119">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="a07da-120">Faça comentários</span><span class="sxs-lookup"><span data-stu-id="a07da-120">Provide feedback</span></span>

<span data-ttu-id="a07da-121">Agradecemos comentários!</span><span class="sxs-lookup"><span data-stu-id="a07da-121">We welcome feedback!</span></span> <span data-ttu-id="a07da-122">Forneça comentários ou Informe qualquer problema no [repositório do GitHub do SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="a07da-122">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>
