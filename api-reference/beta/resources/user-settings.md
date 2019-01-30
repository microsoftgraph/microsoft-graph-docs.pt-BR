---
title: tipo de recurso de configurações
description: 'As configurações do usuário atual. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640508"
---
# <a name="settings-resource-type"></a><span data-ttu-id="2ee40-103">tipo de recurso de configurações</span><span class="sxs-lookup"><span data-stu-id="2ee40-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee40-104">As configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="2ee40-104">The current user settings.</span></span> <span data-ttu-id="2ee40-105">Para saber como obter ou atualizar as configurações de usuário, consulte [obter configurações](../api/user-get-settings.md) e [configurações de atualização](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="2ee40-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="2ee40-106">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="2ee40-106">This resource supports:</span></span>

- <span data-ttu-id="2ee40-107">Verificando se um usuário e a organização do usuário contribuem para detecção de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2ee40-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="2ee40-108">Desativando ou habilitando a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="2ee40-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="2ee40-109">Isso também desabilita documentos no Office me aprofundar.</span><span class="sxs-lookup"><span data-stu-id="2ee40-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="2ee40-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ee40-110">Methods</span></span>
| <span data-ttu-id="2ee40-111">Método</span><span class="sxs-lookup"><span data-stu-id="2ee40-111">Method</span></span>       | <span data-ttu-id="2ee40-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ee40-112">Return Type</span></span>  |<span data-ttu-id="2ee40-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee40-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ee40-114">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="2ee40-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="2ee40-115">Configurações</span><span class="sxs-lookup"><span data-stu-id="2ee40-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="2ee40-116">Obtenha as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="2ee40-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="2ee40-117">Atualizar configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="2ee40-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="2ee40-118">Configurações</span><span class="sxs-lookup"><span data-stu-id="2ee40-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="2ee40-119">Atualize as configurações de usuário atual.</span><span class="sxs-lookup"><span data-stu-id="2ee40-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ee40-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ee40-120">Properties</span></span>

| <span data-ttu-id="2ee40-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ee40-121">Property</span></span>     | <span data-ttu-id="2ee40-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ee40-122">Type</span></span>   |<span data-ttu-id="2ee40-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee40-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ee40-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="2ee40-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="2ee40-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee40-125">Boolean</span></span>|<span data-ttu-id="2ee40-126">API [de tendências](insights-trending.md) quando definido como true, o acesso de representante para o usuário está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="2ee40-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="2ee40-127">Quando definido como true, documentos no Office de me aprofundar o usuário estão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="2ee40-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="2ee40-128">Quando definido como true, a relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business é afetado.</span><span class="sxs-lookup"><span data-stu-id="2ee40-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="2ee40-129">Os usuários podem controlar essa configuração no [Office me aprofundar](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="2ee40-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="2ee40-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="2ee40-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="2ee40-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee40-131">Boolean</span></span>|<span data-ttu-id="2ee40-132">Reflete a [configuração de nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlar o acesso de representante para a [análise de tendências](insights-trending.md) API.</span><span class="sxs-lookup"><span data-stu-id="2ee40-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="2ee40-133">Quando definido como true, a organização não tem acesso ao Office me aprofundar.</span><span class="sxs-lookup"><span data-stu-id="2ee40-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="2ee40-134">A relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de descoberta no OneDrive for Business será afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="2ee40-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="2ee40-135">Essa configuração é somente leitura e só pode ser alterada pelos administradores, no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="2ee40-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ee40-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ee40-136">JSON representation</span></span>

<span data-ttu-id="2ee40-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ee40-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
