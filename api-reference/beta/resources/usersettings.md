---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d44c21c1d41214aec8661fe696179b6976765b4
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897782"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="eb419-103">Tipo de recurso de configurações do usuário (UserSettings)</span><span class="sxs-lookup"><span data-stu-id="eb419-103">userSettings resource type</span></span>

<span data-ttu-id="eb419-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb419-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb419-105">Configurações que representam as preferências de um usuário para [idiomas regionais e idioma](../resources/regionalandlanguagesettings.md), para o [agendamento de turnos](../resources/shiftpreferences.md)e para o [insights e a descoberta de conteúdo](../resources/officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="eb419-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), and for [insights and content discovery](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="eb419-106">Gerenciar preferências baseadas em localidade do usuário:</span><span class="sxs-lookup"><span data-stu-id="eb419-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="eb419-107">Determinar a qual idioma e a formatação regional um usuário prefere exibir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eb419-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="eb419-108">Atualização de preferências de idioma e formatação regional do usuário.</span><span class="sxs-lookup"><span data-stu-id="eb419-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="eb419-109">Gerenciar preferências de turno de trabalho do usuário:</span><span class="sxs-lookup"><span data-stu-id="eb419-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="eb419-110">Verificar se um usuário pode ser atribuído a turnos em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="eb419-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="eb419-111">Atualização de preferências de turno do usuário.</span><span class="sxs-lookup"><span data-stu-id="eb419-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="eb419-112">Habilitar a descoberta de conteúdo e insights centrados em documentos:</span><span class="sxs-lookup"><span data-stu-id="eb419-112">Enable discovery of content and document-centric insights:</span></span>
  - <span data-ttu-id="eb419-113">Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="eb419-113">Checking whether a user and the user's organization contribute to content discovery.</span></span>
  - <span data-ttu-id="eb419-114">Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="eb419-114">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="eb419-115">Isso também desabilita documentos no Office Delve.</span><span class="sxs-lookup"><span data-stu-id="eb419-115">This also disables documents in Office Delve.</span></span>

<span data-ttu-id="eb419-116">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="eb419-116">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="eb419-117">Esse ponto de extremidade só funciona com usuários.</span><span class="sxs-lookup"><span data-stu-id="eb419-117">This endpoint works only with users.</span></span> <span data-ttu-id="eb419-118">Você não pode usar esse ponto de extremidade com os contatos.</span><span class="sxs-lookup"><span data-stu-id="eb419-118">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="eb419-119">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb419-119">Methods</span></span>
| <span data-ttu-id="eb419-120">Método</span><span class="sxs-lookup"><span data-stu-id="eb419-120">Method</span></span>       | <span data-ttu-id="eb419-121">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb419-121">Return Type</span></span>  |<span data-ttu-id="eb419-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb419-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb419-123">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="eb419-123">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="eb419-124">userSettings</span><span class="sxs-lookup"><span data-stu-id="eb419-124">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="eb419-125">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="eb419-125">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="eb419-126">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="eb419-126">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="eb419-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="eb419-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="eb419-128">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="eb419-128">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb419-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb419-129">Properties</span></span>

| <span data-ttu-id="eb419-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb419-130">Property</span></span>     | <span data-ttu-id="eb419-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb419-131">Type</span></span>   |<span data-ttu-id="eb419-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb419-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb419-133">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="eb419-133">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="eb419-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb419-134">Boolean</span></span>|<span data-ttu-id="eb419-135">O acesso delegado à API [mais popular](insights-trending.md) do usuário é desabilitada quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="eb419-135">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="eb419-136">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="eb419-136">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="eb419-137">Quando definido como true, a relevância do conteúdo exibido no Microsoft 365, por exemplo, em sites sugeridos na página inicial do SharePoint, e o modo de exibição de descoberta no OneDrive for Business são afetados.</span><span class="sxs-lookup"><span data-stu-id="eb419-137">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="eb419-138">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="eb419-138">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="eb419-139">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="eb419-139">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="eb419-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb419-140">Boolean</span></span>|<span data-ttu-id="eb419-141">Reflete a [configuração do nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="eb419-141">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="eb419-142">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="eb419-142">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="eb419-143">A relevância do conteúdo exibido no Microsoft 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business, é afetada para toda a organização.</span><span class="sxs-lookup"><span data-stu-id="eb419-143">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="eb419-144">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="eb419-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb419-145">Relações</span><span class="sxs-lookup"><span data-stu-id="eb419-145">Relationships</span></span>

| <span data-ttu-id="eb419-146">Relação</span><span class="sxs-lookup"><span data-stu-id="eb419-146">Relationship</span></span> | <span data-ttu-id="eb419-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb419-147">Type</span></span> | <span data-ttu-id="eb419-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb419-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eb419-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="eb419-149">shiftPreferences</span></span>|[<span data-ttu-id="eb419-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="eb419-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="eb419-151">As preferências de mudança para o usuário.</span><span class="sxs-lookup"><span data-stu-id="eb419-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="eb419-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="eb419-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="eb419-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="eb419-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="eb419-154">As preferências do usuário para os idiomas, a localidade regional e a formatação de data/hora.</span><span class="sxs-lookup"><span data-stu-id="eb419-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb419-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb419-155">JSON representation</span></span>

<span data-ttu-id="eb419-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb419-156">Here is a JSON representation of the resource.</span></span>
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
