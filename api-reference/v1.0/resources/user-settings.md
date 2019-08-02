---
title: tipo de recurso de configurações
description: 'As configurações do usuário atual. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a1cf4deb5da03daeb9d90e03ea63fa069a0701e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033520"
---
# <a name="settings-resource-type"></a><span data-ttu-id="ec72b-103">tipo de recurso de configurações</span><span class="sxs-lookup"><span data-stu-id="ec72b-103">settings resource type</span></span>

<span data-ttu-id="ec72b-104">As configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="ec72b-104">The current user settings.</span></span> <span data-ttu-id="ec72b-105">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/user-get-settings.md) e [Atualizar configurações](../api/user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="ec72b-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="ec72b-106">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="ec72b-106">This resource supports:</span></span>

- <span data-ttu-id="ec72b-107">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="ec72b-108">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="ec72b-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="ec72b-109">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="ec72b-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="ec72b-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="ec72b-110">Methods</span></span>
| <span data-ttu-id="ec72b-111">Método</span><span class="sxs-lookup"><span data-stu-id="ec72b-111">Method</span></span>       | <span data-ttu-id="ec72b-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ec72b-112">Return Type</span></span>  |<span data-ttu-id="ec72b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec72b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec72b-114">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="ec72b-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="ec72b-115">configurações</span><span class="sxs-lookup"><span data-stu-id="ec72b-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="ec72b-116">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="ec72b-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="ec72b-117">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="ec72b-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="ec72b-118">configurações</span><span class="sxs-lookup"><span data-stu-id="ec72b-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="ec72b-119">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="ec72b-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec72b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec72b-120">Properties</span></span>

| <span data-ttu-id="ec72b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec72b-121">Property</span></span>     | <span data-ttu-id="ec72b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec72b-122">Type</span></span>   |<span data-ttu-id="ec72b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec72b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec72b-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="ec72b-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="ec72b-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec72b-125">Boolean</span></span>|<span data-ttu-id="ec72b-126">O acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="ec72b-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="ec72b-127">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="ec72b-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="ec72b-128">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada quando definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="ec72b-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="ec72b-129">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/pt-BR/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="ec72b-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="ec72b-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="ec72b-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="ec72b-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="ec72b-131">Boolean</span></span>|<span data-ttu-id="ec72b-132">Reflete a [configuração do nível de organização](https://support.office.com/pt-BR/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="ec72b-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="ec72b-133">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="ec72b-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="ec72b-134">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="ec72b-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="ec72b-135">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="ec72b-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ec72b-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec72b-136">JSON representation</span></span>

<span data-ttu-id="ec72b-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec72b-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
