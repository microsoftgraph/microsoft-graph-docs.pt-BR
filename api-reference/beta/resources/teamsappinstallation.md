---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66cf31f21a105934181aee5e506cc2215f9ce7a9
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663902"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="a9ffc-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a9ffc-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="a9ffc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9ffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ffc-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="a9ffc-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="a9ffc-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="a9ffc-107">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="a9ffc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a9ffc-108">Methods</span></span>

| <span data-ttu-id="a9ffc-109">Método</span><span class="sxs-lookup"><span data-stu-id="a9ffc-109">Method</span></span>       | <span data-ttu-id="a9ffc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a9ffc-110">Return Type</span></span>  |<span data-ttu-id="a9ffc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ffc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9ffc-112">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="a9ffc-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="a9ffc-113">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="a9ffc-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="a9ffc-114">Listar aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="a9ffc-115">Obter o aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="a9ffc-115">Get app installed in team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="a9ffc-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a9ffc-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="a9ffc-117">Obtenha o aplicativo especificado instalado em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="a9ffc-118">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="a9ffc-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="a9ffc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-119">None</span></span> | <span data-ttu-id="a9ffc-120">Adicionar (instalar) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="a9ffc-121">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="a9ffc-121">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="a9ffc-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-122">None</span></span> | <span data-ttu-id="a9ffc-123">Atualize o aplicativo instalado em uma equipe para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-123">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="a9ffc-124">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="a9ffc-124">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="a9ffc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-125">None</span></span> | <span data-ttu-id="a9ffc-126">Remova (desinstale) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-126">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="a9ffc-127">Lista de aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9ffc-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="a9ffc-128">Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="a9ffc-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="a9ffc-129">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a9ffc-130">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9ffc-130">Get app installed for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="a9ffc-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a9ffc-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="a9ffc-132">Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="a9ffc-133">Adicionar o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9ffc-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="a9ffc-134">Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a9ffc-135">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9ffc-135">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="a9ffc-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-136">None</span></span> | <span data-ttu-id="a9ffc-137">Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-137">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="a9ffc-138">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="a9ffc-138">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="a9ffc-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-139">None</span></span> | <span data-ttu-id="a9ffc-140">Remova (desinstale) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-140">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="a9ffc-141">Listar aplicativos no chat</span><span class="sxs-lookup"><span data-stu-id="a9ffc-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="a9ffc-142">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="a9ffc-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="a9ffc-143">Listar aplicativos instalados em um chat.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="a9ffc-144">Obter o aplicativo instalado no chat</span><span class="sxs-lookup"><span data-stu-id="a9ffc-144">Get app installed in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="a9ffc-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a9ffc-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="a9ffc-146">Obtenha o aplicativo especificado instalado em um chat.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="a9ffc-147">Adicionar aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="a9ffc-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="a9ffc-148">Adicionar (instalar) um aplicativo a um chat.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="a9ffc-149">Atualizar aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="a9ffc-149">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="a9ffc-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-150">None</span></span> | <span data-ttu-id="a9ffc-151">Atualize o aplicativo instalado em um chat para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-151">Upgrade the app installed in a chat to the latest version.</span></span>|
|[<span data-ttu-id="a9ffc-152">Remover aplicativo de chat</span><span class="sxs-lookup"><span data-stu-id="a9ffc-152">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="a9ffc-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9ffc-153">None</span></span> | <span data-ttu-id="a9ffc-154">Remova (desinstale) o aplicativo de um chat.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-154">Remove (uninstall) app from a chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9ffc-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9ffc-155">Properties</span></span>

| <span data-ttu-id="a9ffc-156">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9ffc-156">Property</span></span>            | <span data-ttu-id="a9ffc-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9ffc-157">Type</span></span>     | <span data-ttu-id="a9ffc-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ffc-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a9ffc-159">id</span><span class="sxs-lookup"><span data-stu-id="a9ffc-159">id</span></span>                  | <span data-ttu-id="a9ffc-160">string</span><span class="sxs-lookup"><span data-stu-id="a9ffc-160">string</span></span>   | <span data-ttu-id="a9ffc-161">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="a9ffc-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a9ffc-162">Relações</span><span class="sxs-lookup"><span data-stu-id="a9ffc-162">Relationships</span></span>

| <span data-ttu-id="a9ffc-163">Relação</span><span class="sxs-lookup"><span data-stu-id="a9ffc-163">Relationship</span></span>   | <span data-ttu-id="a9ffc-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9ffc-164">Type</span></span>    | <span data-ttu-id="a9ffc-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ffc-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a9ffc-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a9ffc-166">teamsApp</span></span>|[<span data-ttu-id="a9ffc-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a9ffc-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="a9ffc-168">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-168">The app that is installed.</span></span> |
|<span data-ttu-id="a9ffc-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a9ffc-169">teamsAppDefinition</span></span>|[<span data-ttu-id="a9ffc-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a9ffc-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="a9ffc-171">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9ffc-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9ffc-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9ffc-172">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="a9ffc-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="a9ffc-173">See also</span></span>

- [<span data-ttu-id="a9ffc-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a9ffc-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a9ffc-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a9ffc-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a9ffc-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a9ffc-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="a9ffc-177">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a9ffc-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


