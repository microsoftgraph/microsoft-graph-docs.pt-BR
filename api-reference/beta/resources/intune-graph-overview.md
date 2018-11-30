---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037983"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="a10be-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a10be-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="a10be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a10be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a10be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a10be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a10be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a10be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a10be-107">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="a10be-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="a10be-108">Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.</span><span class="sxs-lookup"><span data-stu-id="a10be-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="a10be-109">Uso da API do Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="a10be-109">Using the Intune Graph API</span></span>

<span data-ttu-id="a10be-110">Intune fornece dados para o Microsoft Graph da mesma forma, como outros serviços em nuvem, com a navegação de informações e a relação de entidade avançada.</span><span class="sxs-lookup"><span data-stu-id="a10be-110">Intune provides data into the Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="a10be-111">Use o Microsoft Graph para combinar informações de outros serviços e Intune construa ricas aplicativos de serviço entre para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="a10be-111">  Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="a10be-112">Veja um exemplo de como determinar se um aplicativo está instalado no dispositivo de um usuário:</span><span class="sxs-lookup"><span data-stu-id="a10be-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="a10be-113">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="a10be-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="a10be-114">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="a10be-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="a10be-115">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="a10be-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a><span data-ttu-id="a10be-116">Usando escopos de permissão do gráfico</span><span class="sxs-lookup"><span data-stu-id="a10be-116">Using Graph permission scopes</span></span>

<span data-ttu-id="a10be-117">Gráfico Microsof controla o acesso a recursos usando escopos de permissão.</span><span class="sxs-lookup"><span data-stu-id="a10be-117">Microsof Graph controls access to resources using permission scopes.</span></span> <span data-ttu-id="a10be-118">Como desenvolvedor, você deve especificar os escopos de permissão necessários para acessar os recursos do Intune.</span><span class="sxs-lookup"><span data-stu-id="a10be-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="a10be-119">Normalmente, você deve especificar os escopos de permissão necessários no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a10be-119">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="a10be-120">Para saber mais, veja [Escopos de permissão do Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) e [Escopos de permissão do Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="a10be-120">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a><span data-ttu-id="a10be-121">Usar o sumário no site do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a10be-121">To use the Table of Contents on the Microsoft Graph site</span></span>
  
<span data-ttu-id="a10be-122">Você pode procurar o sumário (no painel esquerdo do site) para localizar as partes da documentação do Intune gráfico API e recursos que você deseja ver.</span><span class="sxs-lookup"><span data-stu-id="a10be-122">You can browse the Table of Contents (in the left pane of the site) to find the parts of the Intune Graph API and resource documentation you want to see.</span></span>

1. <span data-ttu-id="a10be-123">Clique em **Referência /Beta** para abrir os docs beta.</span><span class="sxs-lookup"><span data-stu-id="a10be-123">Click **/Beta Reference** to open the beta docs.</span></span>
2. <span data-ttu-id="a10be-124">Role para baixo e clique em **Intune**.</span><span class="sxs-lookup"><span data-stu-id="a10be-124">Scroll down and click **Intune**.</span></span>
3. <span data-ttu-id="a10be-125">Continue a clicar em subseções abaixo **Intune** das partes da API você</span><span class="sxs-lookup"><span data-stu-id="a10be-125">Continue to click subsections below **Intune** for the parts of the API you</span></span> 
