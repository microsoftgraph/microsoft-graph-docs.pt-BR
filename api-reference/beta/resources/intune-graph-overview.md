---
title: Uso da API do Graph para Intune - API do Microsoft Graph
description: Lista a API do Microsoft Graph para Terminais do Intune (REST) que você pode usar para gerenciar sua organização de locatários e seus dispositivos, aplicativos, acesso e recursos.
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: d18e86708e43c4945037ad8494eb613c0695c21a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601689"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="bafe9-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bafe9-103">Working with Intune in Microsoft Graph</span></span>  

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> <span data-ttu-id="bafe9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bafe9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bafe9-105">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="bafe9-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="bafe9-106">Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Microsoft Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.</span><span class="sxs-lookup"><span data-stu-id="bafe9-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

<span data-ttu-id="bafe9-107">Todas as APIs do Microsoft Graph beta para o Intune são testadas e validadas pela equipe do Intune antes de serem implantadas.</span><span class="sxs-lookup"><span data-stu-id="bafe9-107">All Microsoft Graph beta APIs for Intune are tested and validated by the Intune team before they're deployed.</span></span> <span data-ttu-id="bafe9-108">Para as últimas mudanças nas APIs, consulte o [changelog](/graph/changelog).</span><span class="sxs-lookup"><span data-stu-id="bafe9-108">For the latest API changes, see the [changelog](/graph/changelog).</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="bafe9-109">Uso da API do Microsoft Graph no Intune</span><span class="sxs-lookup"><span data-stu-id="bafe9-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="bafe9-110">O Intune fornece dados para o Microsoft Graph da mesma forma que outros serviços em nuvem, com rica informação de entidade e navegação de relacionamento.</span><span class="sxs-lookup"><span data-stu-id="bafe9-110">Intune provides data into Microsoft Graph in the same way that other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="bafe9-111">Use o Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados com serviços variados para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="bafe9-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="bafe9-112">O exemplo a seguir mostra como determinar se um aplicativo está instalado no dispositivo de um usuário:</span><span class="sxs-lookup"><span data-stu-id="bafe9-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="bafe9-113">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="bafe9-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="bafe9-114">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="bafe9-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="bafe9-115">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="bafe9-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="bafe9-116">Uso das permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bafe9-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="bafe9-117">O Microsoft Graph controla o acesso aos recursos por meio de permissões.</span><span class="sxs-lookup"><span data-stu-id="bafe9-117">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="bafe9-118">Como desenvolvedor, você deve especificar as permissões necessárias para acessar os recursos do Intune.</span><span class="sxs-lookup"><span data-stu-id="bafe9-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="bafe9-119">Normalmente, você deve especificar as permissões no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bafe9-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="bafe9-120">Para saber mais, confira [Referência de permissões do Microsoft Graph](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bafe9-120">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="bafe9-121">Novidades</span><span class="sxs-lookup"><span data-stu-id="bafe9-121">What's new</span></span>
<span data-ttu-id="bafe9-122">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="bafe9-122">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bafe9-123">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bafe9-123">Next Steps</span></span>

- <span data-ttu-id="bafe9-124">Saiba [como usar o Azure AD](/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="bafe9-124">Learn [how to use Azure AD](/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="bafe9-125">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bafe9-125">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
