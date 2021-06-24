---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a16ab96bb04f6d7dfc4f9ceff29f49dc7d348d23
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108870"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="a244b-103">Tipo de recurso de configurações do usuário (UserSettings)</span><span class="sxs-lookup"><span data-stu-id="a244b-103">userSettings resource type</span></span>

<span data-ttu-id="a244b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a244b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a244b-105">Configurações que representam as preferências de um usuário para [localidades](../resources/regionalandlanguagesettings.md)regionais e idiomas, para agendamento de [turnos,](../resources/shiftpreferences.md)para Delve e para insights [de item.](../resources/officegraphinsights.md)</span><span class="sxs-lookup"><span data-stu-id="a244b-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), for Delve and for [item insights](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="a244b-106">Gerenciar as preferências baseadas na localidade do usuário:</span><span class="sxs-lookup"><span data-stu-id="a244b-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="a244b-107">Determinando com qual idioma e formatação regional um usuário prefere exibir aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a244b-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="a244b-108">Atualizando o idioma de um usuário e as preferências de formatação regional.</span><span class="sxs-lookup"><span data-stu-id="a244b-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="a244b-109">Gerenciar as preferências de turno de trabalho do usuário:</span><span class="sxs-lookup"><span data-stu-id="a244b-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="a244b-110">Verificar se um usuário pode ser atribuído a turnos em um cronograma.</span><span class="sxs-lookup"><span data-stu-id="a244b-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="a244b-111">Atualizando as preferências de turno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a244b-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="a244b-112">Gerenciar Delve acessibilidade:</span><span class="sxs-lookup"><span data-stu-id="a244b-112">Manage Delve accessibility:</span></span>
  - <span data-ttu-id="a244b-113">Verificar se um usuário e a organização do usuário têm acesso a Office Delve.</span><span class="sxs-lookup"><span data-stu-id="a244b-113">Checking whether a user and the user's organization have access to Office Delve.</span></span>
  - <span data-ttu-id="a244b-114">Desabilitando ou habilitando documentos em Office Delve para usuários específicos.</span><span class="sxs-lookup"><span data-stu-id="a244b-114">Disabling or enabling documents in Office Delve for specific users.</span></span> 

<span data-ttu-id="a244b-115">Configure a visibilidade dos [insights de itemInsights](../resources/iteminsights.md) e [de horas de reunião.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="a244b-115">Configure the visibility of [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span> <span data-ttu-id="a244b-116">ItemInsights são derivados entre usuários e outros itens (como documentos ou sites) em Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="a244b-116">ItemInsights are derived between users and other items (such as documents or sites) in Microsoft 365:</span></span>
  - <span data-ttu-id="a244b-117">Verificando se os insights de item e horário de reunião de um usuário estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="a244b-117">Checking whether a user's item and meeting hours insights are enabled.</span></span>
  - <span data-ttu-id="a244b-118">Desabilitando ou habilitando informações de item e horas de reunião para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="a244b-118">Disabling or enabling item and meeting hours insights for specific user.</span></span>

<span data-ttu-id="a244b-119">Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="a244b-119">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="a244b-120">Esse ponto de extremidade só funciona com usuários.</span><span class="sxs-lookup"><span data-stu-id="a244b-120">This endpoint works only with users.</span></span> <span data-ttu-id="a244b-121">Você não pode usar esse ponto de extremidade com os contatos.</span><span class="sxs-lookup"><span data-stu-id="a244b-121">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="a244b-122">Métodos</span><span class="sxs-lookup"><span data-stu-id="a244b-122">Methods</span></span>
| <span data-ttu-id="a244b-123">Método</span><span class="sxs-lookup"><span data-stu-id="a244b-123">Method</span></span>       | <span data-ttu-id="a244b-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a244b-124">Return Type</span></span>  |<span data-ttu-id="a244b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a244b-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a244b-126">Obter configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="a244b-126">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="a244b-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="a244b-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="a244b-128">Obter as configurações de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="a244b-128">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="a244b-129">Atualizar as configurações de usuário</span><span class="sxs-lookup"><span data-stu-id="a244b-129">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="a244b-130">userSettings</span><span class="sxs-lookup"><span data-stu-id="a244b-130">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="a244b-131">Atualize as configurações do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="a244b-131">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="a244b-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a244b-132">Properties</span></span>

| <span data-ttu-id="a244b-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a244b-133">Property</span></span>     | <span data-ttu-id="a244b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a244b-134">Type</span></span>   |<span data-ttu-id="a244b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a244b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a244b-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="a244b-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="a244b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="a244b-137">Boolean</span></span>|<span data-ttu-id="a244b-138">Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros.</span><span class="sxs-lookup"><span data-stu-id="a244b-138">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="a244b-139">Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="a244b-139">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="a244b-140">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="a244b-140">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="a244b-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="a244b-141">Boolean</span></span>|<span data-ttu-id="a244b-142">Reflete a configuração [Office Delve nível da organização.](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)</span><span class="sxs-lookup"><span data-stu-id="a244b-142">Reflects the [Office Delve organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff).</span></span> <span data-ttu-id="a244b-143">A organização não tem acesso ao Office Delve quando definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="a244b-143">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="a244b-144">Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span><span class="sxs-lookup"><span data-stu-id="a244b-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a244b-145">Relações</span><span class="sxs-lookup"><span data-stu-id="a244b-145">Relationships</span></span>

| <span data-ttu-id="a244b-146">Relação</span><span class="sxs-lookup"><span data-stu-id="a244b-146">Relationship</span></span> | <span data-ttu-id="a244b-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="a244b-147">Type</span></span> | <span data-ttu-id="a244b-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="a244b-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a244b-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="a244b-149">shiftPreferences</span></span>|[<span data-ttu-id="a244b-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="a244b-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="a244b-151">As preferências de turno para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a244b-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="a244b-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="a244b-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="a244b-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="a244b-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="a244b-154">Preferências do usuário para idiomas, localidade regional e formatação de data/hora.</span><span class="sxs-lookup"><span data-stu-id="a244b-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |
|<span data-ttu-id="a244b-155">itemInsights</span><span class="sxs-lookup"><span data-stu-id="a244b-155">itemInsights</span></span>|[<span data-ttu-id="a244b-156">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="a244b-156">userInsightsSettings</span></span>](userinsightssettings.md)| <span data-ttu-id="a244b-157">As configurações do usuário para a visibilidade das percepções de hora de reunião e percepções derivadas entre um usuário e outros itens no Microsoft 365, como documentos ou sites.</span><span class="sxs-lookup"><span data-stu-id="a244b-157">The user's settings for the visibility of meeting hour insights, and insights derived between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="a244b-158">[Obter userInsightsSettings](../api/userinsightssettings-get.md) por meio dessa propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="a244b-158">[Get userInsightsSettings](../api/userinsightssettings-get.md) through this navigation property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a244b-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a244b-159">JSON representation</span></span>

<span data-ttu-id="a244b-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a244b-160">Here is a JSON representation of the resource.</span></span>
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


