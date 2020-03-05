---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b3852afc1a4ff790f6be92e39b359ec55230c2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519495"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="cab9e-103">Tipo de recurso de configurações do usuário (UserSettings)</span><span class="sxs-lookup"><span data-stu-id="cab9e-103">userSettings resource type</span></span>

<span data-ttu-id="cab9e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cab9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cab9e-105">As atuais configurações de usuário para descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cab9e-105">The current user settings for content discovery.</span></span> <span data-ttu-id="cab9e-106">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="cab9e-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="cab9e-107">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="cab9e-107">This resource supports:</span></span>

- <span data-ttu-id="cab9e-108">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cab9e-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="cab9e-109">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="cab9e-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="cab9e-110">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="cab9e-110">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="cab9e-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="cab9e-111">Methods</span></span>
| <span data-ttu-id="cab9e-112">Método</span><span class="sxs-lookup"><span data-stu-id="cab9e-112">Method</span></span>       | <span data-ttu-id="cab9e-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cab9e-113">Return Type</span></span>  |<span data-ttu-id="cab9e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab9e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cab9e-115">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="cab9e-115">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="cab9e-116">userSettings</span><span class="sxs-lookup"><span data-stu-id="cab9e-116">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="cab9e-117">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="cab9e-117">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="cab9e-118">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="cab9e-118">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="cab9e-119">userSettings</span><span class="sxs-lookup"><span data-stu-id="cab9e-119">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="cab9e-120">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="cab9e-120">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="cab9e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cab9e-121">Properties</span></span>

| <span data-ttu-id="cab9e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cab9e-122">Property</span></span>     | <span data-ttu-id="cab9e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab9e-123">Type</span></span>   |<span data-ttu-id="cab9e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab9e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cab9e-125">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="cab9e-125">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="cab9e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="cab9e-126">Boolean</span></span>|<span data-ttu-id="cab9e-127">O acesso delegado à API [mais popular](insights-trending.md) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="cab9e-127">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="cab9e-128">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="cab9e-128">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="cab9e-129">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada quando definida como verdadeira.</span><span class="sxs-lookup"><span data-stu-id="cab9e-129">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="cab9e-130">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="cab9e-130">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="cab9e-131">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="cab9e-131">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="cab9e-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="cab9e-132">Boolean</span></span>|<span data-ttu-id="cab9e-133">Reflete a [configuração do nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="cab9e-133">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="cab9e-134">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="cab9e-134">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="cab9e-135">A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="cab9e-135">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="cab9e-136">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="cab9e-136">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="cab9e-137">Relações</span><span class="sxs-lookup"><span data-stu-id="cab9e-137">Relationships</span></span>

| <span data-ttu-id="cab9e-138">Relação</span><span class="sxs-lookup"><span data-stu-id="cab9e-138">Relationship</span></span> | <span data-ttu-id="cab9e-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab9e-139">Type</span></span> | <span data-ttu-id="cab9e-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cab9e-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cab9e-141">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="cab9e-141">shiftPreferences</span></span>|[<span data-ttu-id="cab9e-142">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="cab9e-142">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="cab9e-143">As preferências de mudança para o usuário.</span><span class="sxs-lookup"><span data-stu-id="cab9e-143">The shift preferences for the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cab9e-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cab9e-144">JSON representation</span></span>

<span data-ttu-id="cab9e-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cab9e-145">Here is a JSON representation of the resource.</span></span>
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
