---
title: Uso da API do Graph para Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para pontos de extremidade do Intune (REST), você pode usar para gerenciar a organização do locatário, seus dispositivos, aplicativos, acesso e recursos.
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 883fce914176b2e08d49e4de414cc7c09776714a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941188"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="4d379-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4d379-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="4d379-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d379-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d379-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d379-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d379-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/pt-BR/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d379-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/pt-BR/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="4d379-107">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="4d379-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="4d379-108">Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Microsoft Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](https://docs.microsoft.com/pt-BR/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.</span><span class="sxs-lookup"><span data-stu-id="4d379-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/pt-BR/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="4d379-109">Uso da API do Microsoft Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="4d379-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="4d379-110">O Intune fornece dados para o Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com informações valiosas sobre entidades e navegação de relacionamentos.</span><span class="sxs-lookup"><span data-stu-id="4d379-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="4d379-111">Use o Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados com serviços variados para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="4d379-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="4d379-112">O exemplo a seguir mostra como determinar se um aplicativo está instalado no dispositivo de um usuário:</span><span class="sxs-lookup"><span data-stu-id="4d379-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="4d379-113">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="4d379-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="4d379-114">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="4d379-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="4d379-115">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="4d379-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="4d379-116">Uso das permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4d379-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="4d379-117">O Microsoft Graph controla o acesso a recursos por meio de permissões.</span><span class="sxs-lookup"><span data-stu-id="4d379-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="4d379-118">Como desenvolvedor, você deve especificar as permissões necessárias para acessar os recursos do Intune.</span><span class="sxs-lookup"><span data-stu-id="4d379-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="4d379-119">Normalmente, você deve especificar as permissões no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4d379-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="4d379-120">Para saber mais, confira [Referência de permissões do Microsoft Graph](https://docs.microsoft.com/pt-BR/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d379-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/pt-BR/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4d379-121">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="4d379-121">Next Steps</span></span>

- <span data-ttu-id="4d379-122">Saiba [como usar o Azure AD](https://docs.microsoft.com/pt-BR/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="4d379-122">Learn [how to use Azure AD](https://docs.microsoft.com/pt-BR/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="4d379-123">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="4d379-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

