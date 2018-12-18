---
title: Uso da API do Graph para Intune
description: " Implantações híbridas de Intune não são suportadas. "
author: tfitzmac
ms.openlocfilehash: 9ac823fcc1e3c09bfedc57d9caf4901c95aa9142
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332729"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="8d42d-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8d42d-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="8d42d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8d42d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8d42d-105">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="8d42d-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="8d42d-106">Para cenários de gerenciamento (MDM) do dispositivo móvel, a API do Microsoft Graph para Intune oferece suporte a implantações autônomo; Não há suporte para Intune [implantações híbridas](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) .</span><span class="sxs-lookup"><span data-stu-id="8d42d-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="8d42d-107">Usando a API do Microsoft Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="8d42d-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="8d42d-108">O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos.</span><span class="sxs-lookup"><span data-stu-id="8d42d-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="8d42d-109">Use a API do Microsoft Graph para combinar informações de outros serviços e Intune construa ricas aplicativos de serviço entre para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="8d42d-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="8d42d-110">O exemplo a seguir mostra como você pode determinar se um aplicativo está instalado em um dispositivo do usuário:</span><span class="sxs-lookup"><span data-stu-id="8d42d-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="8d42d-111">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="8d42d-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="8d42d-112">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="8d42d-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="8d42d-113">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="8d42d-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="8d42d-114">Utilização das permissões</span><span class="sxs-lookup"><span data-stu-id="8d42d-114">Using permissions</span></span>

<span data-ttu-id="8d42d-115">A API do Microsoft Graph controla o acesso aos recursos por meio de permissões.</span><span class="sxs-lookup"><span data-stu-id="8d42d-115">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="8d42d-116">Como um desenvolvedor, você deve especificar as permissões que necessárias para acessar recursos Intune.</span><span class="sxs-lookup"><span data-stu-id="8d42d-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="8d42d-117">Normalmente, você deve especificar as permissões no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8d42d-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="8d42d-118">Para obter mais informações, consulte [referência de permissões do Microsoft Graph](https://docs.microsoft.com/en-us/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d42d-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8d42d-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8d42d-119">Next Steps</span></span>

- <span data-ttu-id="8d42d-120">Saiba [como usar o Windows Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="8d42d-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="8d42d-121">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8d42d-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
