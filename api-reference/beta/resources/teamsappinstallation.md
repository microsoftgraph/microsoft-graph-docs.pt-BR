---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f5775514eb242f540bc6740d8e21620448f2d280
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563636"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="b1218-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1218-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="b1218-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1218-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1218-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="b1218-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="b1218-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="b1218-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="b1218-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1218-107">Methods</span></span>

| <span data-ttu-id="b1218-108">Método</span><span class="sxs-lookup"><span data-stu-id="b1218-108">Method</span></span>       | <span data-ttu-id="b1218-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1218-109">Return Type</span></span>  |<span data-ttu-id="b1218-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1218-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1218-111">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="b1218-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="b1218-112">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="b1218-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="b1218-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b1218-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="b1218-114">Obter o aplicativo instalado em uma equipe</span><span class="sxs-lookup"><span data-stu-id="b1218-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="b1218-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1218-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="b1218-116">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b1218-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="b1218-117">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="b1218-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) |<span data-ttu-id="b1218-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1218-118">None</span></span> | <span data-ttu-id="b1218-119">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b1218-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="b1218-120">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="b1218-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="b1218-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1218-121">None</span></span> | <span data-ttu-id="b1218-122">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b1218-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="b1218-123">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="b1218-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="b1218-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1218-124">None</span></span> | <span data-ttu-id="b1218-125">Atualiza para a versão mais recente do aplicativo instalado no Team.</span><span class="sxs-lookup"><span data-stu-id="b1218-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="b1218-126">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="b1218-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="b1218-127">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="b1218-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="b1218-128">Lista os aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1218-128">Lists apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="b1218-129">Obtém o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="b1218-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="b1218-130">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1218-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="b1218-131">Lista o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1218-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="b1218-132">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="b1218-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | | <span data-ttu-id="b1218-133">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1218-133">Adds (installs) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="b1218-134">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="b1218-134">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="b1218-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1218-135">None</span></span> | <span data-ttu-id="b1218-136">Remove (desinstala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1218-136">Removes (uninstalls) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="b1218-137">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="b1218-137">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="b1218-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1218-138">None</span></span> | <span data-ttu-id="b1218-139">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1218-139">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1218-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1218-140">Properties</span></span>

| <span data-ttu-id="b1218-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1218-141">Property</span></span>            | <span data-ttu-id="b1218-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1218-142">Type</span></span>     | <span data-ttu-id="b1218-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1218-143">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b1218-144">id</span><span class="sxs-lookup"><span data-stu-id="b1218-144">id</span></span>                  | <span data-ttu-id="b1218-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1218-145">string</span></span>   | <span data-ttu-id="b1218-146">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="b1218-146">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="b1218-147">Relações</span><span class="sxs-lookup"><span data-stu-id="b1218-147">Relationships</span></span>

| <span data-ttu-id="b1218-148">Relação</span><span class="sxs-lookup"><span data-stu-id="b1218-148">Relationship</span></span>   | <span data-ttu-id="b1218-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1218-149">Type</span></span>    | <span data-ttu-id="b1218-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1218-150">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b1218-151">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1218-151">teamsApp</span></span>|[<span data-ttu-id="b1218-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1218-152">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="b1218-153">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="b1218-153">The app that is installed.</span></span> |
|<span data-ttu-id="b1218-154">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1218-154">teamsAppDefinition</span></span>|[<span data-ttu-id="b1218-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1218-155">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="b1218-156">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1218-156">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1218-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1218-157">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="b1218-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="b1218-158">See also</span></span>

- [<span data-ttu-id="b1218-159">teamsApp</span><span class="sxs-lookup"><span data-stu-id="b1218-159">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="b1218-160">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="b1218-160">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="b1218-161">teamsTab</span><span class="sxs-lookup"><span data-stu-id="b1218-161">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="b1218-162">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b1218-162">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


