---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: jpettere
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85a1a9556a5bc02224c8add5e97bc6cbd442cf77
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721873"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="eefad-103">Tipo de recurso de configurações do usuário (UserSettings)</span><span class="sxs-lookup"><span data-stu-id="eefad-103">userSettings resource type</span></span>

<span data-ttu-id="eefad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eefad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eefad-105">As atuais configurações de usuário para descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="eefad-105">The current user settings for content discovery.</span></span>
<span data-ttu-id="eefad-106">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="eefad-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="eefad-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="eefad-107">This resource supports:</span></span>

- <span data-ttu-id="eefad-108">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="eefad-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="eefad-109">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="eefad-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="eefad-110">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="eefad-110">This also disables documents in Office Delve.</span></span>

> [!NOTE]
> <span data-ttu-id="eefad-111">Esse ponto de extremidade só funciona com usuários.</span><span class="sxs-lookup"><span data-stu-id="eefad-111">This endpoint works only with users.</span></span> <span data-ttu-id="eefad-112">Você não pode usar esse ponto de extremidade com os contatos.</span><span class="sxs-lookup"><span data-stu-id="eefad-112">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="eefad-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="eefad-113">Methods</span></span>
| <span data-ttu-id="eefad-114">Método</span><span class="sxs-lookup"><span data-stu-id="eefad-114">Method</span></span>       | <span data-ttu-id="eefad-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eefad-115">Return Type</span></span>  |<span data-ttu-id="eefad-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="eefad-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eefad-117">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="eefad-117">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="eefad-118">userSettings</span><span class="sxs-lookup"><span data-stu-id="eefad-118">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="eefad-119">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="eefad-119">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="eefad-120">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="eefad-120">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="eefad-121">userSettings</span><span class="sxs-lookup"><span data-stu-id="eefad-121">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="eefad-122">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="eefad-122">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="eefad-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eefad-123">Properties</span></span>

| <span data-ttu-id="eefad-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eefad-124">Property</span></span>     | <span data-ttu-id="eefad-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="eefad-125">Type</span></span>   |<span data-ttu-id="eefad-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="eefad-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eefad-127">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="eefad-127">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="eefad-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="eefad-128">Boolean</span></span>|<span data-ttu-id="eefad-129">O acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="eefad-129">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="eefad-130">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="eefad-130">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="eefad-131">Quando definida como verdadeira, a relevância do conteúdo exibido no Microsoft 365, como em sites Sugeridos na Página Inicial do Microsoft Office SharePoint Online e o modo de exibição Descobrir no OneDrive for Business é afetada.</span><span class="sxs-lookup"><span data-stu-id="eefad-131">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="eefad-132">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="eefad-132">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="eefad-133">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="eefad-133">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="eefad-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="eefad-134">Boolean</span></span>|<span data-ttu-id="eefad-135">Reflete a [configuração do nível de organização](https://support.office.com/pt-BR/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="eefad-135">Reflects the [organization level setting](https://support.office.com/pt-BR/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="eefad-136">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="eefad-136">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="eefad-137">A relevância do conteúdo exibido no Microsoft 365, como em sites Sugeridos na Página Inicial do Microsoft Office SharePoint Online e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="eefad-137">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="eefad-138">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="eefad-138">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eefad-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eefad-139">JSON representation</span></span>

<span data-ttu-id="eefad-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eefad-140">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```

