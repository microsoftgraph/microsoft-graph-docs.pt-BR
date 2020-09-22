---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a74323dc8a5e5907ea8a91553537fc8259acea6c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046584"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="a994f-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a994f-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="a994f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a994f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a994f-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="a994f-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="a994f-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="a994f-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="a994f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a994f-107">Methods</span></span>

| <span data-ttu-id="a994f-108">Método</span><span class="sxs-lookup"><span data-stu-id="a994f-108">Method</span></span>       | <span data-ttu-id="a994f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a994f-109">Return Type</span></span>  |<span data-ttu-id="a994f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a994f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a994f-111">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="a994f-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="a994f-112">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="a994f-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a994f-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="a994f-114">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="a994f-114">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="a994f-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a994f-115">None</span></span> | <span data-ttu-id="a994f-116">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a994f-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="a994f-117">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="a994f-117">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="a994f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a994f-118">None</span></span> | <span data-ttu-id="a994f-119">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a994f-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="a994f-120">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="a994f-120">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="a994f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a994f-121">None</span></span> | <span data-ttu-id="a994f-122">Atualiza para a versão mais recente do aplicativo instalado no Team.</span><span class="sxs-lookup"><span data-stu-id="a994f-122">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="a994f-123">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="a994f-123">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="a994f-124">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-124">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="a994f-125">Lista os aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a994f-125">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a994f-126">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="a994f-126">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="a994f-127">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a994f-127">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a994f-128">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="a994f-128">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="a994f-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a994f-129">None</span></span> | <span data-ttu-id="a994f-130">Remove (desinstala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a994f-130">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a994f-131">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="a994f-131">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="a994f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a994f-132">None</span></span> | <span data-ttu-id="a994f-133">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a994f-133">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="a994f-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a994f-134">Properties</span></span>

| <span data-ttu-id="a994f-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a994f-135">Property</span></span>            | <span data-ttu-id="a994f-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a994f-136">Type</span></span>     | <span data-ttu-id="a994f-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a994f-137">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a994f-138">id</span><span class="sxs-lookup"><span data-stu-id="a994f-138">id</span></span>                  | <span data-ttu-id="a994f-139">string</span><span class="sxs-lookup"><span data-stu-id="a994f-139">string</span></span>   | <span data-ttu-id="a994f-140">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="a994f-140">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a994f-141">Relações</span><span class="sxs-lookup"><span data-stu-id="a994f-141">Relationships</span></span>

| <span data-ttu-id="a994f-142">Relação</span><span class="sxs-lookup"><span data-stu-id="a994f-142">Relationship</span></span>   | <span data-ttu-id="a994f-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="a994f-143">Type</span></span>    | <span data-ttu-id="a994f-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="a994f-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a994f-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a994f-145">teamsApp</span></span>|[<span data-ttu-id="a994f-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a994f-146">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="a994f-147">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="a994f-147">The app that is installed.</span></span> |
|<span data-ttu-id="a994f-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a994f-148">teamsAppDefinition</span></span>|[<span data-ttu-id="a994f-149">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a994f-149">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="a994f-150">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a994f-150">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a994f-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a994f-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a994f-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="a994f-152">See also</span></span>

- [<span data-ttu-id="a994f-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a994f-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a994f-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a994f-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a994f-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a994f-155">teamsTab</span></span>](../resources/teamstab.md)

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


