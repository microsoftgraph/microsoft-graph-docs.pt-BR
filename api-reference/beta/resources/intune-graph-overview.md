---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 1db77aceaab82e869fc540d2b29cce17ddba100f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911949"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="03423-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="03423-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="03423-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="03423-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03423-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03423-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="03423-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="03423-107">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="03423-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="03423-108">Para cenários de gerenciamento (MDM) do dispositivo móvel, a API do Microsoft Graph para Intune oferece suporte a implantações autônomo; Não há suporte para Intune [implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) .</span><span class="sxs-lookup"><span data-stu-id="03423-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="03423-109">Usando a API do Microsoft Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="03423-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="03423-110">Intune fornece dados para o Microsoft Graph da mesma forma, como outros serviços em nuvem, com a navegação de informações e a relação de entidade avançada.</span><span class="sxs-lookup"><span data-stu-id="03423-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="03423-111">Use o Microsoft Graph para combinar informações de outros serviços e Intune construa ricas aplicativos de serviço entre para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="03423-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="03423-112">O exemplo a seguir mostra como você pode determinar se um aplicativo está instalado em um dispositivo do usuário:</span><span class="sxs-lookup"><span data-stu-id="03423-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="03423-113">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="03423-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="03423-114">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="03423-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="03423-115">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="03423-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="03423-116">Usando permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="03423-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="03423-117">Gráfico de Microsof controla o acesso aos recursos por meio de permissões.</span><span class="sxs-lookup"><span data-stu-id="03423-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="03423-118">Como um desenvolvedor, você deve especificar as permissões que necessárias para acessar recursos Intune.</span><span class="sxs-lookup"><span data-stu-id="03423-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="03423-119">Normalmente, você deve especificar as permissões no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03423-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="03423-120">Para obter mais informações, consulte [referência de permissões do Microsoft Graph](https://docs.microsoft.com/en-us/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03423-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="03423-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="03423-121">Next Steps</span></span>

- <span data-ttu-id="03423-122">Saiba [como usar o Windows Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="03423-122">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="03423-123">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="03423-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

