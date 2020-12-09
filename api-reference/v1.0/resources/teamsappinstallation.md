---
title: tipo de recurso teamsAppInstallation
description: Representa um teamsApp instalado em uma equipe ou o escopo pessoal de um usuário.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c872d41ebc09978d9dc54ac01d82cb33258541d
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607032"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="efd80-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="efd80-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="efd80-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="efd80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efd80-105">Representa um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md) ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="efd80-105">Represents a [teamsApp](teamsapp.md) installed in a [team](team.md) or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="efd80-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer escopo pessoal do usuário ou da equipe ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="efd80-106">Any bots that are part of the app will become part of any team or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="efd80-107">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="efd80-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="efd80-108">Methods</span><span class="sxs-lookup"><span data-stu-id="efd80-108">Methods</span></span>

| <span data-ttu-id="efd80-109">Método</span><span class="sxs-lookup"><span data-stu-id="efd80-109">Method</span></span>       | <span data-ttu-id="efd80-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="efd80-110">Return Type</span></span>  |<span data-ttu-id="efd80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd80-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efd80-112">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="efd80-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="efd80-113">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="efd80-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="efd80-114">Listar aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="efd80-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="efd80-115">Obter o aplicativo instalado em uma equipe</span><span class="sxs-lookup"><span data-stu-id="efd80-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="efd80-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="efd80-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="efd80-117">Obtenha o aplicativo especificado instalado em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="efd80-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="efd80-118">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="efd80-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="efd80-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd80-119">None</span></span> | <span data-ttu-id="efd80-120">Adicionar (instalar) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="efd80-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="efd80-121">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="efd80-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="efd80-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd80-122">None</span></span> | <span data-ttu-id="efd80-123">Remova (desinstale) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="efd80-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="efd80-124">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="efd80-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="efd80-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd80-125">None</span></span> | <span data-ttu-id="efd80-126">Atualize o aplicativo instalado em uma equipe para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="efd80-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="efd80-127">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="efd80-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="efd80-128">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="efd80-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="efd80-129">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efd80-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="efd80-130">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="efd80-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="efd80-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="efd80-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="efd80-132">Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efd80-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="efd80-133">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="efd80-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="efd80-134">Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efd80-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="efd80-135">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="efd80-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="efd80-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd80-136">None</span></span> | <span data-ttu-id="efd80-137">Remova (desinstale) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efd80-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="efd80-138">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="efd80-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="efd80-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd80-139">None</span></span> | <span data-ttu-id="efd80-140">Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="efd80-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|


## <a name="properties"></a><span data-ttu-id="efd80-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efd80-141">Properties</span></span>

| <span data-ttu-id="efd80-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efd80-142">Property</span></span>            | <span data-ttu-id="efd80-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="efd80-143">Type</span></span>     | <span data-ttu-id="efd80-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd80-144">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="efd80-145">id</span><span class="sxs-lookup"><span data-stu-id="efd80-145">id</span></span>                  | <span data-ttu-id="efd80-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efd80-146">string</span></span>   | <span data-ttu-id="efd80-147">Uma ID exclusiva (não a ID do aplicativo Teams).</span><span class="sxs-lookup"><span data-stu-id="efd80-147">A unique ID (not the Teams app ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="efd80-148">Relações</span><span class="sxs-lookup"><span data-stu-id="efd80-148">Relationships</span></span>

| <span data-ttu-id="efd80-149">Relação</span><span class="sxs-lookup"><span data-stu-id="efd80-149">Relationship</span></span>   | <span data-ttu-id="efd80-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="efd80-150">Type</span></span>    | <span data-ttu-id="efd80-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd80-151">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="efd80-152">teamsApp</span><span class="sxs-lookup"><span data-stu-id="efd80-152">teamsApp</span></span>|[<span data-ttu-id="efd80-153">teamsApp</span><span class="sxs-lookup"><span data-stu-id="efd80-153">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="efd80-154">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="efd80-154">The app that is installed.</span></span> |
|<span data-ttu-id="efd80-155">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="efd80-155">teamsAppDefinition</span></span>|[<span data-ttu-id="efd80-156">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="efd80-156">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="efd80-157">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="efd80-157">The details of this version of the app.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="efd80-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efd80-158">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="efd80-159">Confira também</span><span class="sxs-lookup"><span data-stu-id="efd80-159">See also</span></span>

- [<span data-ttu-id="efd80-160">teamsApp</span><span class="sxs-lookup"><span data-stu-id="efd80-160">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="efd80-161">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="efd80-161">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="efd80-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="efd80-162">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="efd80-163">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="efd80-163">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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

