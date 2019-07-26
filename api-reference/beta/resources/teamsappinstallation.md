---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e1246616b7a3d76c6170a02286a2cde2a15d3a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908506"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="e824c-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="e824c-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e824c-104">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="e824c-104">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="e824c-105">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="e824c-105">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="e824c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e824c-106">Methods</span></span>

| <span data-ttu-id="e824c-107">Método</span><span class="sxs-lookup"><span data-stu-id="e824c-107">Method</span></span>       | <span data-ttu-id="e824c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e824c-108">Return Type</span></span>  |<span data-ttu-id="e824c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e824c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e824c-110">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="e824c-110">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="e824c-111">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e824c-111">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e824c-112">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="e824c-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="e824c-113">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="e824c-113">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="e824c-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e824c-114">None</span></span> | <span data-ttu-id="e824c-115">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="e824c-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="e824c-116">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="e824c-116">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="e824c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e824c-117">None</span></span> | <span data-ttu-id="e824c-118">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="e824c-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="e824c-119">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="e824c-119">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="e824c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e824c-120">None</span></span> | <span data-ttu-id="e824c-121">Atualiza para a versão mais recente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e824c-121">Upgrades to the latest version of the app.</span></span>|
|[<span data-ttu-id="e824c-122">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="e824c-122">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="e824c-123">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="e824c-123">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="e824c-124">Lista os aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e824c-124">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e824c-125">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="e824c-125">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="e824c-126">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e824c-126">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e824c-127">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="e824c-127">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="e824c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e824c-128">None</span></span> | <span data-ttu-id="e824c-129">Remove (desinstala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e824c-129">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="e824c-130">Atualizar aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="e824c-130">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="e824c-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e824c-131">None</span></span> | <span data-ttu-id="e824c-132">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e824c-132">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="e824c-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e824c-133">Properties</span></span>

| <span data-ttu-id="e824c-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e824c-134">Property</span></span>            | <span data-ttu-id="e824c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e824c-135">Type</span></span>     | <span data-ttu-id="e824c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e824c-136">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e824c-137">id</span><span class="sxs-lookup"><span data-stu-id="e824c-137">id</span></span>                  | <span data-ttu-id="e824c-138">string</span><span class="sxs-lookup"><span data-stu-id="e824c-138">string</span></span>   | <span data-ttu-id="e824c-139">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="e824c-139">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e824c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e824c-140">Relationships</span></span>

| <span data-ttu-id="e824c-141">Relação</span><span class="sxs-lookup"><span data-stu-id="e824c-141">Relationship</span></span>   | <span data-ttu-id="e824c-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="e824c-142">Type</span></span>    | <span data-ttu-id="e824c-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="e824c-143">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e824c-144">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e824c-144">teamsApp</span></span>|[<span data-ttu-id="e824c-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e824c-145">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="e824c-146">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="e824c-146">The app that is installed.</span></span> |
|<span data-ttu-id="e824c-147">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e824c-147">teamsAppDefinition</span></span>|[<span data-ttu-id="e824c-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e824c-148">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="e824c-149">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e824c-149">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e824c-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e824c-150">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="e824c-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="e824c-151">See also</span></span>

- [<span data-ttu-id="e824c-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e824c-152">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="e824c-153">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="e824c-153">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="e824c-154">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e824c-154">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
