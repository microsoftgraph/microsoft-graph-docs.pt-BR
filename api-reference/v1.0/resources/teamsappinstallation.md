---
title: tipo de recurso teamsAppInstallation
description: Representa um teamsApp instalado em uma equipe ou o escopo pessoal de um usuário.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da55c4cf7b20558258493c69c46e2b26107f4aed
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660069"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="46a24-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="46a24-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="46a24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46a24-105">Representa um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md) ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="46a24-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="46a24-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer escopo pessoal do usuário ou da equipe ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="46a24-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="46a24-107">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="46a24-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="46a24-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="46a24-108">Methods</span></span>

| <span data-ttu-id="46a24-109">Método</span><span class="sxs-lookup"><span data-stu-id="46a24-109">Method</span></span>       | <span data-ttu-id="46a24-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46a24-110">Return Type</span></span>  |<span data-ttu-id="46a24-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a24-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46a24-112">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="46a24-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="46a24-113">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="46a24-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="46a24-114">Listar aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="46a24-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="46a24-115">Obter o aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="46a24-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="46a24-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="46a24-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="46a24-117">Obtenha o aplicativo especificado instalado em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="46a24-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="46a24-118">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="46a24-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="46a24-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46a24-119">None</span></span> | <span data-ttu-id="46a24-120">Adicionar (instalar) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="46a24-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="46a24-121">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="46a24-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="46a24-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46a24-122">None</span></span> | <span data-ttu-id="46a24-123">Atualize o aplicativo instalado em uma equipe para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="46a24-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="46a24-124">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="46a24-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="46a24-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46a24-125">None</span></span> | <span data-ttu-id="46a24-126">Remova (desinstale) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="46a24-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="46a24-127">Lista de aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="46a24-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="46a24-128">Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="46a24-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="46a24-129">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="46a24-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="46a24-130">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="46a24-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="46a24-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="46a24-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="46a24-132">Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="46a24-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="46a24-133">Adicionar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="46a24-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="46a24-134">Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="46a24-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="46a24-135">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="46a24-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="46a24-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46a24-136">None</span></span> | <span data-ttu-id="46a24-137">Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="46a24-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="46a24-138">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="46a24-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="46a24-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46a24-139">None</span></span> | <span data-ttu-id="46a24-140">Remova (desinstale) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="46a24-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|


## <a name="properties"></a><span data-ttu-id="46a24-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46a24-141">Properties</span></span>

| <span data-ttu-id="46a24-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46a24-142">Property</span></span>            | <span data-ttu-id="46a24-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="46a24-143">Type</span></span>     | <span data-ttu-id="46a24-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a24-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="46a24-145">id</span><span class="sxs-lookup"><span data-stu-id="46a24-145">id</span></span>                  | <span data-ttu-id="46a24-146">string</span><span class="sxs-lookup"><span data-stu-id="46a24-146">string</span></span>   | <span data-ttu-id="46a24-147">Uma ID exclusiva (não a ID do aplicativo Teams).</span><span class="sxs-lookup"><span data-stu-id="46a24-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="46a24-148">Relações</span><span class="sxs-lookup"><span data-stu-id="46a24-148">Relationships</span></span>

| <span data-ttu-id="46a24-149">Relação</span><span class="sxs-lookup"><span data-stu-id="46a24-149">Relationship</span></span>   | <span data-ttu-id="46a24-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="46a24-150">Type</span></span>    | <span data-ttu-id="46a24-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="46a24-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="46a24-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="46a24-152">teamsApp</span></span>|[<span data-ttu-id="46a24-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="46a24-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="46a24-154">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="46a24-154">The app that is installed.</span></span> |
|<span data-ttu-id="46a24-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="46a24-155">teamsAppDefinition</span></span>|[<span data-ttu-id="46a24-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="46a24-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="46a24-157">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46a24-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="46a24-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46a24-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="46a24-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="46a24-159">See also</span></span>

- [<span data-ttu-id="46a24-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="46a24-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="46a24-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="46a24-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="46a24-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="46a24-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="46a24-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="46a24-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

