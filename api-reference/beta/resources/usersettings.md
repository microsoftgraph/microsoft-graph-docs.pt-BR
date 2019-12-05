---
title: tipo de recurso UserSettings
description: 'As configurações de usuário atuais para descoberta de conteúdo. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0168ee426bb9c03d7a53add2d1842a498c930330
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844250"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="4a27e-103">tipo de recurso UserSettings</span><span class="sxs-lookup"><span data-stu-id="4a27e-103">userSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a27e-104">As configurações de usuário atuais para descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4a27e-104">The current user settings for content discovery.</span></span> <span data-ttu-id="4a27e-105">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="4a27e-105">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="4a27e-106">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="4a27e-106">This resource supports:</span></span>

- <span data-ttu-id="4a27e-107">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4a27e-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="4a27e-108">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="4a27e-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="4a27e-109">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="4a27e-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="4a27e-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a27e-110">Methods</span></span>
| <span data-ttu-id="4a27e-111">Método</span><span class="sxs-lookup"><span data-stu-id="4a27e-111">Method</span></span>       | <span data-ttu-id="4a27e-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a27e-112">Return Type</span></span>  |<span data-ttu-id="4a27e-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a27e-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a27e-114">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="4a27e-114">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="4a27e-115">userSettings</span><span class="sxs-lookup"><span data-stu-id="4a27e-115">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="4a27e-116">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="4a27e-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="4a27e-117">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="4a27e-117">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="4a27e-118">userSettings</span><span class="sxs-lookup"><span data-stu-id="4a27e-118">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="4a27e-119">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="4a27e-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a27e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a27e-120">Properties</span></span>

| <span data-ttu-id="4a27e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a27e-121">Property</span></span>     | <span data-ttu-id="4a27e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a27e-122">Type</span></span>   |<span data-ttu-id="4a27e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a27e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a27e-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="4a27e-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="4a27e-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a27e-125">Boolean</span></span>|<span data-ttu-id="4a27e-126">O acesso delegado à API [mais popular](insights-trending.md) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="4a27e-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="4a27e-127">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="4a27e-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="4a27e-128">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada quando definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="4a27e-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="4a27e-129">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="4a27e-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="4a27e-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="4a27e-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="4a27e-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a27e-131">Boolean</span></span>|<span data-ttu-id="4a27e-132">Reflete a [configuração do nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="4a27e-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="4a27e-133">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="4a27e-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="4a27e-134">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="4a27e-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="4a27e-135">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="4a27e-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a27e-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a27e-136">JSON representation</span></span>

<span data-ttu-id="4a27e-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a27e-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
