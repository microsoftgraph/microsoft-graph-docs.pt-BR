---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
ms.openlocfilehash: 23f6550fca708b64357b7b5132a2a42060cfa4bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003399"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="f28c6-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f28c6-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="f28c6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f28c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f28c6-105">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="f28c6-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="f28c6-106">Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.</span><span class="sxs-lookup"><span data-stu-id="f28c6-106">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="f28c6-107">Uso da API do Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="f28c6-107">Using the Intune Graph API</span></span>

<span data-ttu-id="f28c6-108">O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos.</span><span class="sxs-lookup"><span data-stu-id="f28c6-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="f28c6-109">Use a API do Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados com serviços variados para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="f28c6-109">  Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="f28c6-110">Veja um exemplo de como determinar se um aplicativo está instalado no dispositivo de um usuário:</span><span class="sxs-lookup"><span data-stu-id="f28c6-110">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="f28c6-111">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="f28c6-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="f28c6-112">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="f28c6-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="f28c6-113">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="f28c6-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a><span data-ttu-id="f28c6-114">Usar escopos de permissão</span><span class="sxs-lookup"><span data-stu-id="f28c6-114">Using permission scopes</span></span>

<span data-ttu-id="f28c6-115">A API do Microsoft Graph controla o acesso a recursos por meio de escopos de permissão.</span><span class="sxs-lookup"><span data-stu-id="f28c6-115">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="f28c6-116">Como desenvolvedor, você deve especificar os escopos de permissão necessários para acessar os recursos do Intune.</span><span class="sxs-lookup"><span data-stu-id="f28c6-116">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="f28c6-117">Normalmente, você deve especificar os escopos de permissão necessários no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f28c6-117">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="f28c6-118">Para saber mais, veja [Escopos de permissão do Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) e [Escopos de permissão do Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="f28c6-118">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="next-steps"></a><span data-ttu-id="f28c6-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f28c6-119">Next Steps</span></span>

- <span data-ttu-id="f28c6-120">Saiba [como usar o Windows Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="f28c6-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="f28c6-121">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do gráfico para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f28c6-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use Graph API for Intune in context of working examples.</span></span>