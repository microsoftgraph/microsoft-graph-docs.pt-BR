---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9b34450f29ccb1fb02cf1751c78f312c71fdefc9
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606950"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="c823c-103">tipo de recurso teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c823c-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="c823c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c823c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c823c-105">Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="c823c-105">A [teamsApp](teamsapp.md) installed in a [team](team.md), a [chat](chat.md), or the personal scope of a [user](user.md).</span></span> <span data-ttu-id="c823c-106">Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.</span><span class="sxs-lookup"><span data-stu-id="c823c-106">Any bots that are part of the app will become part of any team, chat, or user's personal scope that the app is added to.</span></span>

> [!NOTE]
> <span data-ttu-id="c823c-107">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="c823c-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="methods"></a><span data-ttu-id="c823c-108">Methods</span><span class="sxs-lookup"><span data-stu-id="c823c-108">Methods</span></span>

| <span data-ttu-id="c823c-109">Método</span><span class="sxs-lookup"><span data-stu-id="c823c-109">Method</span></span>       | <span data-ttu-id="c823c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c823c-110">Return Type</span></span>  |<span data-ttu-id="c823c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c823c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c823c-112">Listar aplicativos instalados no Team</span><span class="sxs-lookup"><span data-stu-id="c823c-112">List apps installed in team</span></span>](../api/team-list-installedapps.md) | <span data-ttu-id="c823c-113">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="c823c-113">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="c823c-114">Listar aplicativos instalados em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c823c-114">List apps installed in a team.</span></span>|
|[<span data-ttu-id="c823c-115">Obter o aplicativo instalado em uma equipe</span><span class="sxs-lookup"><span data-stu-id="c823c-115">Get app installed in a team</span></span>](../api/team-get-installedapps.md) | [<span data-ttu-id="c823c-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c823c-116">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="c823c-117">Obtenha o aplicativo especificado instalado em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c823c-117">Get the specified app installed in a team.</span></span>|
|[<span data-ttu-id="c823c-118">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="c823c-118">Add app to team</span></span>](../api/team-post-installedapps.md) |<span data-ttu-id="c823c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-119">None</span></span> | <span data-ttu-id="c823c-120">Adicionar (instalar) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c823c-120">Add (install) an app to a team.</span></span>|
|[<span data-ttu-id="c823c-121">Remover aplicativo da equipe</span><span class="sxs-lookup"><span data-stu-id="c823c-121">Remove app from team</span></span>](../api/team-delete-installedapps.md) | <span data-ttu-id="c823c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-122">None</span></span> | <span data-ttu-id="c823c-123">Remova (desinstale) um aplicativo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="c823c-123">Remove (uninstall) an app from a team.</span></span>|
|[<span data-ttu-id="c823c-124">Atualizar aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="c823c-124">Upgrade app installed in team</span></span>](../api/team-teamsappinstallation-upgrade.md) | <span data-ttu-id="c823c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-125">None</span></span> | <span data-ttu-id="c823c-126">Atualize o aplicativo instalado em uma equipe para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="c823c-126">Upgrade the app installed in a team to the latest version.</span></span>|
|[<span data-ttu-id="c823c-127">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="c823c-127">List apps installed for user</span></span>](../api/userteamwork-list-installedapps.md) | <span data-ttu-id="c823c-128">coleção [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="c823c-128">[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) collection</span></span> | <span data-ttu-id="c823c-129">Listar aplicativos instalados no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c823c-129">List apps installed in the personal scope of a user.</span></span>|
|[<span data-ttu-id="c823c-130">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="c823c-130">Get the installed app for user</span></span>](../api/userteamwork-get-installedapps.md)| [<span data-ttu-id="c823c-131">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c823c-131">userScopeTeamsAppInstallation</span></span>](userscopeteamsappinstallation.md) | <span data-ttu-id="c823c-132">Obtenha o aplicativo especificado instalado no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c823c-132">Get the specified app installed in the personal scope of a user.</span></span> |
|[<span data-ttu-id="c823c-133">Adicionar aplicativo para usuário</span><span class="sxs-lookup"><span data-stu-id="c823c-133">Add app for user</span></span>](../api/userteamwork-post-installedapps.md) | | <span data-ttu-id="c823c-134">Adicionar (instalar) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c823c-134">Add (install) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="c823c-135">Remover o aplicativo para o usuário</span><span class="sxs-lookup"><span data-stu-id="c823c-135">Remove app for user</span></span>](../api/userteamwork-delete-installedapps.md) | <span data-ttu-id="c823c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-136">None</span></span> | <span data-ttu-id="c823c-137">Remova (desinstale) um aplicativo no escopo pessoal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c823c-137">Remove (uninstall) an app in the personal scope of a user.</span></span>|
|[<span data-ttu-id="c823c-138">Atualizar o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="c823c-138">Upgrade app installed for user</span></span>](../api/userteamwork-teamsappinstallation-upgrade.md) | <span data-ttu-id="c823c-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-139">None</span></span> | <span data-ttu-id="c823c-140">Atualize o aplicativo instalado no escopo pessoal de um usuário para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="c823c-140">Upgrade the app installed in the personal scope of a user to the latest version.</span></span>|
|[<span data-ttu-id="c823c-141">Listar aplicativos no chat</span><span class="sxs-lookup"><span data-stu-id="c823c-141">List apps in chat</span></span>](../api/chat-list-installedapps.md) |<span data-ttu-id="c823c-142">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="c823c-142">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="c823c-143">Listar aplicativos instalados em um chat.</span><span class="sxs-lookup"><span data-stu-id="c823c-143">List apps installed in a chat.</span></span>|
|[<span data-ttu-id="c823c-144">Obter aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="c823c-144">Get app in chat</span></span>](../api/chat-get-installedapps.md) | [<span data-ttu-id="c823c-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c823c-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="c823c-146">Obtenha o aplicativo especificado instalado em um chat.</span><span class="sxs-lookup"><span data-stu-id="c823c-146">Get the specified app installed in a chat.</span></span>|
|[<span data-ttu-id="c823c-147">Adicionar aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="c823c-147">Add app in chat</span></span>](../api/chat-post-installedapps.md) | | <span data-ttu-id="c823c-148">Adicionar (instalar) um aplicativo a um chat.</span><span class="sxs-lookup"><span data-stu-id="c823c-148">Add (install) an app to a chat.</span></span>|
|[<span data-ttu-id="c823c-149">Remover aplicativo de chat</span><span class="sxs-lookup"><span data-stu-id="c823c-149">Remove app from chat</span></span>](../api/chat-delete-installedapps.md) | <span data-ttu-id="c823c-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-150">None</span></span> | <span data-ttu-id="c823c-151">Remova (desinstale) o aplicativo de um chat.</span><span class="sxs-lookup"><span data-stu-id="c823c-151">Remove (uninstall) app from a chat.</span></span>|
|[<span data-ttu-id="c823c-152">Atualizar aplicativo no chat</span><span class="sxs-lookup"><span data-stu-id="c823c-152">Upgrade app in chat</span></span>](../api/chat-teamsappinstallation-upgrade.md) | <span data-ttu-id="c823c-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c823c-153">None</span></span> | <span data-ttu-id="c823c-154">Atualize o aplicativo instalado em um chat para a versão mais recente.</span><span class="sxs-lookup"><span data-stu-id="c823c-154">Upgrade the app installed in a chat to the latest version.</span></span>|

## <a name="properties"></a><span data-ttu-id="c823c-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c823c-155">Properties</span></span>

| <span data-ttu-id="c823c-156">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c823c-156">Property</span></span>            | <span data-ttu-id="c823c-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="c823c-157">Type</span></span>     | <span data-ttu-id="c823c-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="c823c-158">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c823c-159">id</span><span class="sxs-lookup"><span data-stu-id="c823c-159">id</span></span>                  | <span data-ttu-id="c823c-160">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c823c-160">string</span></span>   | <span data-ttu-id="c823c-161">Uma ID exclusiva (não a ID de AP da equipe).</span><span class="sxs-lookup"><span data-stu-id="c823c-161">A unique ID (not the team's ap ID).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c823c-162">Relações</span><span class="sxs-lookup"><span data-stu-id="c823c-162">Relationships</span></span>

| <span data-ttu-id="c823c-163">Relação</span><span class="sxs-lookup"><span data-stu-id="c823c-163">Relationship</span></span>   | <span data-ttu-id="c823c-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="c823c-164">Type</span></span>    | <span data-ttu-id="c823c-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="c823c-165">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c823c-166">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c823c-166">teamsApp</span></span>|[<span data-ttu-id="c823c-167">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c823c-167">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="c823c-168">O aplicativo que está instalado.</span><span class="sxs-lookup"><span data-stu-id="c823c-168">The app that is installed.</span></span> |
|<span data-ttu-id="c823c-169">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c823c-169">teamsAppDefinition</span></span>|[<span data-ttu-id="c823c-170">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c823c-170">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="c823c-171">Os detalhes desta versão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c823c-171">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c823c-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c823c-172">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c823c-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="c823c-173">See also</span></span>

- [<span data-ttu-id="c823c-174">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c823c-174">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="c823c-175">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c823c-175">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c823c-176">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c823c-176">teamsTab</span></span>](../resources/teamstab.md)
- [<span data-ttu-id="c823c-177">userScopeTeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c823c-177">userScopeTeamsAppInstallation</span></span>](../resources/userscopeteamsappinstallation.md)

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


