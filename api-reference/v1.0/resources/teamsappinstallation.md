---
title: tipo de recurso teamsAppInstallation
description: Representa um teamsApp instalado em uma equipe ou o escopo pessoal de um usuário.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0d15f65273504b3b7577c875fec69c5a212a8c76
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563748"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="33c3e-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="33c3e-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="33c3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33c3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33c3e-105">Representa um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md) ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="33c3e-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="33c3e-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer escopo pessoal do usuário ou da equipe ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="33c3e-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="33c3e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="33c3e-107">Methods</span></span>

| <span data-ttu-id="33c3e-108">Método</span><span class="sxs-lookup"><span data-stu-id="33c3e-108">Method</span></span>       | <span data-ttu-id="33c3e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33c3e-109">Return Type</span></span>  |<span data-ttu-id="33c3e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c3e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33c3e-111">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="33c3e-111">List apps installed in team</span></span>](../api/teamsappinstallation-list.md) | <span data-ttu-id="33c3e-112">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="33c3e-112">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="33c3e-113">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="33c3e-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="33c3e-114">Obter o aplicativo instalado em uma equipe</span><span class="sxs-lookup"><span data-stu-id="33c3e-114">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="33c3e-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="33c3e-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="33c3e-116">Lista os aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="33c3e-116">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="33c3e-117">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="33c3e-117">Add app to team</span></span>](../api/teamsappinstallation-add.md) | <span data-ttu-id="33c3e-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-118">None</span></span> | <span data-ttu-id="33c3e-119">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="33c3e-119">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="33c3e-120">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="33c3e-120">Remove app from team</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="33c3e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-121">None</span></span> | <span data-ttu-id="33c3e-122">Remove (desinstala) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="33c3e-122">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="33c3e-123">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="33c3e-123">Upgrade app installed in team</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="33c3e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-124">None</span></span> | <span data-ttu-id="33c3e-125">Atualiza para a versão mais recente do aplicativo instalado no Team.</span><span class="sxs-lookup"><span data-stu-id="33c3e-125">Upgrades to the latest version of the app installed in team.</span></span>|
|[<span data-ttu-id="33c3e-126">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="33c3e-126">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md)| <span data-ttu-id="33c3e-127">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="33c3e-127">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="33c3e-128">Lista os aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33c3e-128">Lists apps installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="33c3e-129">Obtém o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="33c3e-129">Gets the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="33c3e-130">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="33c3e-130">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="33c3e-131">Lista o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33c3e-131">Lists the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="33c3e-132">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="33c3e-132">Add app for user</span></span>](../api/userteamwork-add-installedapps.md) | <span data-ttu-id="33c3e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-133">None</span></span> | <span data-ttu-id="33c3e-134">Adiciona (instala) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33c3e-134">Adds (installs) an app in the personal scope of a user.</span></span> |
|[<span data-ttu-id="33c3e-135">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="33c3e-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="33c3e-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-136">None</span></span> | <span data-ttu-id="33c3e-137">Remove (desinstala) um aplicativo do escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33c3e-137">Removes (uninstalls) an app from the personal scope of a user.</span></span> |
|[<span data-ttu-id="33c3e-138">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="33c3e-138">Upgrade app installed for user</span></span>](../api/userteamwork-upgrade-installedapps.md) | <span data-ttu-id="33c3e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33c3e-139">None</span></span> | <span data-ttu-id="33c3e-140">Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="33c3e-140">Upgrades to the latest version of the app installed in the personal scope of a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="33c3e-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33c3e-141">Properties</span></span>

| <span data-ttu-id="33c3e-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33c3e-142">Property</span></span>            | <span data-ttu-id="33c3e-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="33c3e-143">Type</span></span>     | <span data-ttu-id="33c3e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c3e-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="33c3e-145">id</span><span class="sxs-lookup"><span data-stu-id="33c3e-145">id</span></span>                  | <span data-ttu-id="33c3e-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33c3e-146">string</span></span>   | <span data-ttu-id="33c3e-147">Uma ID exclusiva (não a appID do Teams).</span><span class="sxs-lookup"><span data-stu-id="33c3e-147">A unique ID (not the Teams appID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="33c3e-148">Relações</span><span class="sxs-lookup"><span data-stu-id="33c3e-148">Relationships</span></span>

| <span data-ttu-id="33c3e-149">Relação</span><span class="sxs-lookup"><span data-stu-id="33c3e-149">Relationship</span></span>   | <span data-ttu-id="33c3e-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="33c3e-150">Type</span></span>    | <span data-ttu-id="33c3e-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c3e-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="33c3e-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="33c3e-152">teamsApp</span></span>|[<span data-ttu-id="33c3e-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="33c3e-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="33c3e-154">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="33c3e-154">The app that is installed.</span></span> |
|<span data-ttu-id="33c3e-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="33c3e-155">teamsAppDefinition</span></span>|[<span data-ttu-id="33c3e-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="33c3e-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="33c3e-157">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33c3e-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="33c3e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33c3e-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="33c3e-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="33c3e-159">See also</span></span>

- [<span data-ttu-id="33c3e-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="33c3e-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="33c3e-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="33c3e-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="33c3e-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="33c3e-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="33c3e-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="33c3e-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
  "suppressions": []
}-->

