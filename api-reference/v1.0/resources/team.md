---
title: tipo de recurso de equipe
description: 'Uma equipe Teams da Microsoft é uma coleção de canais. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7dff1bb05b2abe604963657d4691766eeeaae4ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976930"
---
# <a name="team-resource-type"></a><span data-ttu-id="2e029-103">tipo de recurso de equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-103">team resource type</span></span>



<span data-ttu-id="2e029-104">Uma equipe Teams da Microsoft é uma coleção de [canais](channel.md).</span><span class="sxs-lookup"><span data-stu-id="2e029-104">A team in Microsoft Teams is a collection of [channels](channel.md).</span></span> <span data-ttu-id="2e029-105">Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2e029-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="2e029-106">Cada equipe é associado um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="2e029-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="2e029-107">O grupo tem a mesma identificação que a equipe - por exemplo, /groups/ {id} / equipe é igual ao /teams/ {id}.</span><span class="sxs-lookup"><span data-stu-id="2e029-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="2e029-108">Para obter mais informações sobre como trabalhar com grupos e membros de equipes, consulte [Use a API do Microsoft Graph REST para trabalhar com as equipes da Microsoft](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2e029-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2e029-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2e029-109">Methods</span></span>

| <span data-ttu-id="2e029-110">Método</span><span class="sxs-lookup"><span data-stu-id="2e029-110">Method</span></span>       | <span data-ttu-id="2e029-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2e029-111">Return Type</span></span>  |<span data-ttu-id="2e029-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e029-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e029-113">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="2e029-114">equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-114">team</span></span>](team.md) | <span data-ttu-id="2e029-115">Criar um novo equipe ou adicione uma equipe a um grupo existente.</span><span class="sxs-lookup"><span data-stu-id="2e029-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="2e029-116">Obtenha a equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="2e029-117">equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-117">team</span></span>](team.md) | <span data-ttu-id="2e029-118">Recupere as propriedades e relacionamentos da equipe especificado.</span><span class="sxs-lookup"><span data-stu-id="2e029-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="2e029-119">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="2e029-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="2e029-120">equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-120">team</span></span>](team.md) |<span data-ttu-id="2e029-121">Atualize as propriedades da equipe especificado.</span><span class="sxs-lookup"><span data-stu-id="2e029-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="2e029-122">Excluir equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="2e029-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e029-123">None</span></span> |<span data-ttu-id="2e029-124">Exclua a equipe e seu grupo associado.</span><span class="sxs-lookup"><span data-stu-id="2e029-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="2e029-125">Equipe de clone</span><span class="sxs-lookup"><span data-stu-id="2e029-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="2e029-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2e029-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2e029-127">Copie a equipe e seu grupo associado.</span><span class="sxs-lookup"><span data-stu-id="2e029-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="2e029-128">Equipe de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="2e029-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="2e029-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2e029-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2e029-130">Colocar a equipe em um estado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e029-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="2e029-131">Equipe de unarchive</span><span class="sxs-lookup"><span data-stu-id="2e029-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="2e029-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="2e029-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="2e029-133">Restaure a equipe em um estado de leitura / gravação.</span><span class="sxs-lookup"><span data-stu-id="2e029-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="2e029-134">Listar suas equipes</span><span class="sxs-lookup"><span data-stu-id="2e029-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="2e029-135">coleção de [equipe](team.md)</span><span class="sxs-lookup"><span data-stu-id="2e029-135">[team](team.md) collection</span></span> | <span data-ttu-id="2e029-136">Liste as equipes que você é um membro de.</span><span class="sxs-lookup"><span data-stu-id="2e029-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="2e029-137">Liste todas as equipes</span><span class="sxs-lookup"><span data-stu-id="2e029-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="2e029-138">Coleção [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="2e029-138">[group](group.md) collection</span></span> | <span data-ttu-id="2e029-139">Liste todos os grupos que possuem equipes.</span><span class="sxs-lookup"><span data-stu-id="2e029-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="2e029-140">Publicar aplicativos à sua organização</span><span class="sxs-lookup"><span data-stu-id="2e029-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="2e029-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2e029-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="2e029-142">Crie aplicativos de equipes visível somente para sua organização.</span><span class="sxs-lookup"><span data-stu-id="2e029-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="2e029-143">Adicionar o aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="2e029-144">teamsappinstallation</span><span class="sxs-lookup"><span data-stu-id="2e029-144">teamsappinstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="2e029-145">Adiciona (instala) um aplicativo para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="2e029-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="2e029-146">Adicionar guia ao canal</span><span class="sxs-lookup"><span data-stu-id="2e029-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="2e029-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2e029-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="2e029-148">Adiciona (instala) uma guia ao canal da equipe.</span><span class="sxs-lookup"><span data-stu-id="2e029-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e029-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e029-149">Properties</span></span>

| <span data-ttu-id="2e029-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e029-150">Property</span></span> | <span data-ttu-id="2e029-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e029-151">Type</span></span>   | <span data-ttu-id="2e029-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e029-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2e029-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-153">funSettings</span></span>|[<span data-ttu-id="2e029-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="2e029-155">Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.</span><span class="sxs-lookup"><span data-stu-id="2e029-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="2e029-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-156">guestSettings</span></span>|[<span data-ttu-id="2e029-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="2e029-158">Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.</span><span class="sxs-lookup"><span data-stu-id="2e029-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="2e029-159">isArchived</span><span class="sxs-lookup"><span data-stu-id="2e029-159">isArchived</span></span>|<span data-ttu-id="2e029-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="2e029-160">Boolean</span></span>|<span data-ttu-id="2e029-161">Se essa equipe está em modo somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2e029-161">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="2e029-162">memberSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-162">memberSettings</span></span>|[<span data-ttu-id="2e029-163">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-163">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="2e029-164">Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.</span><span class="sxs-lookup"><span data-stu-id="2e029-164">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="2e029-165">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-165">messagingSettings</span></span>|[<span data-ttu-id="2e029-166">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="2e029-166">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="2e029-167">Configurações para configurar mensagens e menções na equipe de.</span><span class="sxs-lookup"><span data-stu-id="2e029-167">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="2e029-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="2e029-168">webUrl</span></span>|<span data-ttu-id="2e029-169">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="2e029-169">string (readonly)</span></span> | <span data-ttu-id="2e029-170">Um hiperlink que irão para a equipe no cliente do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2e029-170">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="2e029-171">Esta é a URL que você obtém quando você uma equipe no cliente do Microsoft Teams do mouse em e selecione o **link para a equipe de obter**.</span><span class="sxs-lookup"><span data-stu-id="2e029-171">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="2e029-172">Essa URL deve ser tratado como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="2e029-172">This URL should be treated as an opaque blob, and not parsed.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e029-173">Relações</span><span class="sxs-lookup"><span data-stu-id="2e029-173">Relationships</span></span>

| <span data-ttu-id="2e029-174">Relação</span><span class="sxs-lookup"><span data-stu-id="2e029-174">Relationship</span></span> | <span data-ttu-id="2e029-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e029-175">Type</span></span>   | <span data-ttu-id="2e029-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e029-176">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2e029-177">canais</span><span class="sxs-lookup"><span data-stu-id="2e029-177">channels</span></span>|<span data-ttu-id="2e029-178">coleção de [canal](channel.md)</span><span class="sxs-lookup"><span data-stu-id="2e029-178">[channel](channel.md) collection</span></span>|<span data-ttu-id="2e029-179">A coleção de canais & associadas à equipe de mensagens.</span><span class="sxs-lookup"><span data-stu-id="2e029-179">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="2e029-180">installedApps</span><span class="sxs-lookup"><span data-stu-id="2e029-180">installedApps</span></span>|<span data-ttu-id="2e029-181">coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="2e029-181">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="2e029-182">Os aplicativos instalados nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="2e029-182">The apps installed in this team.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e029-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e029-183">JSON representation</span></span>

<span data-ttu-id="2e029-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e029-184">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{  
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "isArchived": false,
  "webUrl": "https://...longUrl..."
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="2e029-185">Confira também</span><span class="sxs-lookup"><span data-stu-id="2e029-185">See Also</span></span>
- [<span data-ttu-id="2e029-186">Criando um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="2e029-186">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="2e029-187">Usando as APIs de equipes</span><span class="sxs-lookup"><span data-stu-id="2e029-187">Using Teams APIs</span></span>](teams-api-overview.md)
