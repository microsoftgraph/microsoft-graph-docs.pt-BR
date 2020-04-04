---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 43799ef1f4e417f2ebd9fc51c49e4a895f0203b1
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144244"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="0236e-103">Tipo de recurso de configurações do usuário (UserSettings)</span><span class="sxs-lookup"><span data-stu-id="0236e-103">userSettings resource type</span></span>

<span data-ttu-id="0236e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0236e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0236e-105">As atuais configurações de usuário para descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0236e-105">The current user settings for content discovery.</span></span> <span data-ttu-id="0236e-106">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="0236e-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="0236e-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="0236e-107">This resource supports:</span></span>

- <span data-ttu-id="0236e-108">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0236e-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="0236e-109">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="0236e-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="0236e-110">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="0236e-110">This also disables documents in Office Delve.</span></span>

> [!NOTE]
> <span data-ttu-id="0236e-111">Este ponto de extremidade funciona apenas com os usuários.</span><span class="sxs-lookup"><span data-stu-id="0236e-111">This endpoint works only with users.</span></span> <span data-ttu-id="0236e-112">Você não pode usar esse ponto de extremidade com contatos.</span><span class="sxs-lookup"><span data-stu-id="0236e-112">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="0236e-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="0236e-113">Methods</span></span>
| <span data-ttu-id="0236e-114">Método</span><span class="sxs-lookup"><span data-stu-id="0236e-114">Method</span></span>       | <span data-ttu-id="0236e-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0236e-115">Return Type</span></span>  |<span data-ttu-id="0236e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="0236e-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0236e-117">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="0236e-117">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="0236e-118">userSettings</span><span class="sxs-lookup"><span data-stu-id="0236e-118">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="0236e-119">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="0236e-119">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="0236e-120">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="0236e-120">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="0236e-121">userSettings</span><span class="sxs-lookup"><span data-stu-id="0236e-121">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="0236e-122">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="0236e-122">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="0236e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0236e-123">Properties</span></span>

| <span data-ttu-id="0236e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0236e-124">Property</span></span>     | <span data-ttu-id="0236e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0236e-125">Type</span></span>   |<span data-ttu-id="0236e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0236e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0236e-127">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="0236e-127">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="0236e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="0236e-128">Boolean</span></span>|<span data-ttu-id="0236e-129">O acesso delegado à API [mais popular](insights-trending.md) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="0236e-129">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="0236e-130">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="0236e-130">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="0236e-131">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada quando definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="0236e-131">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="0236e-132">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="0236e-132">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="0236e-133">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="0236e-133">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="0236e-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="0236e-134">Boolean</span></span>|<span data-ttu-id="0236e-135">Reflete a [configuração do nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="0236e-135">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="0236e-136">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="0236e-136">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="0236e-137">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="0236e-137">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="0236e-138">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="0236e-138">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0236e-139">Relações</span><span class="sxs-lookup"><span data-stu-id="0236e-139">Relationships</span></span>

| <span data-ttu-id="0236e-140">Relação</span><span class="sxs-lookup"><span data-stu-id="0236e-140">Relationship</span></span> | <span data-ttu-id="0236e-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="0236e-141">Type</span></span> | <span data-ttu-id="0236e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="0236e-142">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0236e-143">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="0236e-143">shiftPreferences</span></span>|[<span data-ttu-id="0236e-144">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="0236e-144">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="0236e-145">As preferências de mudança para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0236e-145">The shift preferences for the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0236e-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0236e-146">JSON representation</span></span>

<span data-ttu-id="0236e-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0236e-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
