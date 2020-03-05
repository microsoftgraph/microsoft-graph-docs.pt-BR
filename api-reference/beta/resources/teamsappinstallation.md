---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10a7d5d58a18e23c47d603e7b05c9981ddfeed76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519908"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="eaf07-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="eaf07-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="eaf07-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eaf07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaf07-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="eaf07-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="eaf07-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="eaf07-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="eaf07-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eaf07-107">Methods</span></span>

| <span data-ttu-id="eaf07-108">Método</span><span class="sxs-lookup"><span data-stu-id="eaf07-108">Method</span></span>       | <span data-ttu-id="eaf07-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eaf07-109">Return Type</span></span>  |<span data-ttu-id="eaf07-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf07-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eaf07-111">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="eaf07-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="eaf07-112">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="eaf07-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="eaf07-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="eaf07-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="eaf07-114">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="eaf07-114">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="eaf07-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf07-115">None</span></span> | <span data-ttu-id="eaf07-116">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="eaf07-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="eaf07-117">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="eaf07-117">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="eaf07-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf07-118">None</span></span> | <span data-ttu-id="eaf07-119">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="eaf07-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="eaf07-120">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="eaf07-120">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="eaf07-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf07-121">None</span></span> | <span data-ttu-id="eaf07-122">Atualiza para a versão mais recente do aplicativo instalado no Team.</span><span class="sxs-lookup"><span data-stu-id="eaf07-122">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="eaf07-123">Lista de aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="eaf07-123">List apps installed for user</span></span>](../api/user-list-teamsappinstallation.md) | <span data-ttu-id="eaf07-124">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="eaf07-124">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="eaf07-125">Lista os aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eaf07-125">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="eaf07-126">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="eaf07-126">Add app for user</span></span>](../api/user-add-teamsappinstallation.md) | | <span data-ttu-id="eaf07-127">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eaf07-127">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="eaf07-128">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="eaf07-128">Remove app for user</span></span>](../api/user-delete-teamsappinstallation.md) | <span data-ttu-id="eaf07-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf07-129">None</span></span> | <span data-ttu-id="eaf07-130">Remove (desinstala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eaf07-130">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="eaf07-131">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="eaf07-131">Upgrade app installed for user</span></span>](../api/user-upgrade-teamsappinstallation.md) | <span data-ttu-id="eaf07-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf07-132">None</span></span> | <span data-ttu-id="eaf07-133">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="eaf07-133">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="eaf07-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaf07-134">Properties</span></span>

| <span data-ttu-id="eaf07-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaf07-135">Property</span></span>            | <span data-ttu-id="eaf07-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf07-136">Type</span></span>     | <span data-ttu-id="eaf07-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf07-137">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="eaf07-138">id</span><span class="sxs-lookup"><span data-stu-id="eaf07-138">id</span></span>                  | <span data-ttu-id="eaf07-139">string</span><span class="sxs-lookup"><span data-stu-id="eaf07-139">string</span></span>   | <span data-ttu-id="eaf07-140">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="eaf07-140">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="eaf07-141">Relações</span><span class="sxs-lookup"><span data-stu-id="eaf07-141">Relationships</span></span>

| <span data-ttu-id="eaf07-142">Relação</span><span class="sxs-lookup"><span data-stu-id="eaf07-142">Relationship</span></span>   | <span data-ttu-id="eaf07-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf07-143">Type</span></span>    | <span data-ttu-id="eaf07-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf07-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eaf07-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eaf07-145">teamsApp</span></span>|[<span data-ttu-id="eaf07-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eaf07-146">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="eaf07-147">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="eaf07-147">The app that is installed.</span></span> |
|<span data-ttu-id="eaf07-148">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="eaf07-148">teamsAppDefinition</span></span>|[<span data-ttu-id="eaf07-149">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="eaf07-149">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="eaf07-150">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eaf07-150">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eaf07-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eaf07-151">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="eaf07-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="eaf07-152">See also</span></span>

- [<span data-ttu-id="eaf07-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="eaf07-153">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="eaf07-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="eaf07-154">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="eaf07-155">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eaf07-155">teamsTab</span></span>](../resources/teamstab.md)

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
