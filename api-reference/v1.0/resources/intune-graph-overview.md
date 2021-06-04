---
title: Uso da API do Graph para Intune
description: " Não há suporte para as implantações híbridas do Intune. "
author: dougeby
localization_priority: Priority
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: baad1c809bfd34dd60bab009b7b83c5fcb46dddf
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732260"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="626c9-103">Trabalhando com o Intune no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="626c9-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="626c9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="626c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="626c9-105">A API do Microsoft Graph para Intune permite o acesso programático a informações do Intune para seu locatário; a API executa as mesmas operações do Intune disponíveis pelo **Portal do Azure**.</span><span class="sxs-lookup"><span data-stu-id="626c9-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="626c9-106">Em cenários de gerenciamento de dispositivo móvel (MDM), a API do Microsoft Graph para Intune oferece suporte a implantações autônomas; não há suporte para[implantações híbridas](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) do Intune.</span><span class="sxs-lookup"><span data-stu-id="626c9-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="626c9-107">Uso da API do Microsoft Graph para Intune</span><span class="sxs-lookup"><span data-stu-id="626c9-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="626c9-108">O Intune fornece dados para a API da Microsoft Graph da mesma forma que outros serviços de nuvem fazem, com valiosas informações sobre entidades e navegação de relacionamentos.</span><span class="sxs-lookup"><span data-stu-id="626c9-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span> <span data-ttu-id="626c9-109">Use a API do Microsoft Graph para combinar informações de outros serviços e do Intune e criar aplicativos avançados de vários serviços para profissionais de TI ou usuários finais.</span><span class="sxs-lookup"><span data-stu-id="626c9-109">Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="626c9-110">O exemplo a seguir mostra como determinar se um aplicativo está instalado no dispositivo de um usuário:</span><span class="sxs-lookup"><span data-stu-id="626c9-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="626c9-111">Obtenha no Azure Active Directory uma lista dos dispositivos registrados de um usuário:</span><span class="sxs-lookup"><span data-stu-id="626c9-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="626c9-112">Em seguida, exiba a lista de aplicativos do seu locatário:</span><span class="sxs-lookup"><span data-stu-id="626c9-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="626c9-113">Obtenha a ID do aplicativo e determine o estado de instalação do aplicativo (e, portanto, do usuário):</span><span class="sxs-lookup"><span data-stu-id="626c9-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="626c9-114">Acessando a API do Microsoft Graph para o Intune</span><span class="sxs-lookup"><span data-stu-id="626c9-114">Accessing the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="626c9-115">O Intune tem suporte para [permissões delegadas](/graph/auth-v2-user) e para [permissões do aplicativo](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="626c9-115">Intune supports both [delegated permissions](/graph/auth-v2-user) and [application permissions](/graph/auth-v2-service).</span></span> <span data-ttu-id="626c9-116">As permissões delegadas e de aplicativo têm suporte para operações de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="626c9-116">Delegated and application permissions support both read and write operations.</span></span> <span data-ttu-id="626c9-117">As permissões delegadas e de aplicativo oferecem suporte a aplicativos de locatário único, bem como a aplicativos multilocatários.</span><span class="sxs-lookup"><span data-stu-id="626c9-117">Delegated and application permissions support both single tenant applications, as well as multi-tenant applications.</span></span> <span data-ttu-id="626c9-118">Para obter mais informações sobre as permissões disponíveis por meio do Microsoft Graph, consulte [referência de permissões do Microsoft Graph](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626c9-118">For more information about the permissions available through Microsoft Graph, see [Microsoft Graph permissions reference](/graph/permissions-reference).</span></span>

## <a name="using-permissions"></a><span data-ttu-id="626c9-119">Usando permissões</span><span class="sxs-lookup"><span data-stu-id="626c9-119">Using permissions</span></span>

<span data-ttu-id="626c9-120">A API do Microsoft Graph controla o acesso a recursos por meio de permissões.</span><span class="sxs-lookup"><span data-stu-id="626c9-120">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="626c9-121">Como desenvolvedor, você deve especificar as permissões necessárias para acessar os recursos do Intune.</span><span class="sxs-lookup"><span data-stu-id="626c9-121">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="626c9-122">Normalmente, você deve especificar as permissões no portal do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="626c9-122">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="626c9-123">Para saber mais, confira [Referência de permissões do Microsoft Graph](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626c9-123">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="626c9-124">Novidades</span><span class="sxs-lookup"><span data-stu-id="626c9-124">What's new</span></span>
<span data-ttu-id="626c9-125">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="626c9-125">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="626c9-126">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="626c9-126">Next Steps</span></span>

- <span data-ttu-id="626c9-127">Saiba [como usar o Azure AD](/intune/intune-graph-apis) para acessar a API do Microsoft Graph para Intune.</span><span class="sxs-lookup"><span data-stu-id="626c9-127">Learn [how to use Azure AD](/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="626c9-128">Explore os [exemplos do PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), que mostram como usar a API do Microsoft Graph para Intune no contexto dos exemplos de trabalho.</span><span class="sxs-lookup"><span data-stu-id="626c9-128">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>