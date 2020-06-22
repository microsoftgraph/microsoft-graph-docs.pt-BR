---
title: tipo de recurso de equipe
description: 'No Microsoft Teams, uma equipe é um conjunto de canais. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 460bbfaa522cf4767d7f35992a4371bf870c8948
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793679"
---
# <a name="team-resource-type"></a><span data-ttu-id="d53a0-103">tipo de recurso de equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-103">team resource type</span></span>

<span data-ttu-id="d53a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d53a0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d53a0-105">No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="d53a0-105">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="d53a0-106">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-106">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="d53a0-107">Cada equipe está associada a um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="d53a0-107">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="d53a0-108">O grupo tem a mesma ID da equipe, por exemplo, /groups/{id}/team é igual a /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="d53a0-108">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="d53a0-109">Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d53a0-109">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d53a0-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="d53a0-110">Methods</span></span>

| <span data-ttu-id="d53a0-111">Método</span><span class="sxs-lookup"><span data-stu-id="d53a0-111">Method</span></span>       | <span data-ttu-id="d53a0-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d53a0-112">Return Type</span></span>  |<span data-ttu-id="d53a0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d53a0-114">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-114">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="d53a0-115">team</span><span class="sxs-lookup"><span data-stu-id="d53a0-115">team</span></span>](team.md) | <span data-ttu-id="d53a0-116">Crie uma nova equipe ou adicione uma equipe a um grupo existente.</span><span class="sxs-lookup"><span data-stu-id="d53a0-116">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="d53a0-117">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-117">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="d53a0-118">team</span><span class="sxs-lookup"><span data-stu-id="d53a0-118">team</span></span>](team.md) | <span data-ttu-id="d53a0-119">Recupere as propriedades e relações da equipe especificada.</span><span class="sxs-lookup"><span data-stu-id="d53a0-119">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="d53a0-120">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-120">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="d53a0-121">team</span><span class="sxs-lookup"><span data-stu-id="d53a0-121">team</span></span>](team.md) |<span data-ttu-id="d53a0-122">Atualize as propriedades da equipe especificada.</span><span class="sxs-lookup"><span data-stu-id="d53a0-122">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="d53a0-123">Excluir equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-123">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="d53a0-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d53a0-124">None</span></span> |<span data-ttu-id="d53a0-125">Exclua a equipe e o grupo associado.</span><span class="sxs-lookup"><span data-stu-id="d53a0-125">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="d53a0-126">Clonar equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-126">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="d53a0-127">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d53a0-127">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d53a0-128">Copie a equipe e o grupo associado.</span><span class="sxs-lookup"><span data-stu-id="d53a0-128">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="d53a0-129">Arquivar equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-129">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="d53a0-130">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d53a0-130">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d53a0-131">Coloque a equipe em um estado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d53a0-131">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="d53a0-132">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-132">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="d53a0-133">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d53a0-133">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="d53a0-134">Restaure a equipe com um estado de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="d53a0-134">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="d53a0-135">Listar suas equipes</span><span class="sxs-lookup"><span data-stu-id="d53a0-135">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="d53a0-136">Coleção [team](team.md)</span><span class="sxs-lookup"><span data-stu-id="d53a0-136">[team](team.md) collection</span></span> | <span data-ttu-id="d53a0-137">Liste as equipes das quais você é membro.</span><span class="sxs-lookup"><span data-stu-id="d53a0-137">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="d53a0-138">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="d53a0-138">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="d53a0-139">Coleção [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="d53a0-139">[group](group.md) collection</span></span> | <span data-ttu-id="d53a0-140">Liste todos os grupos que têm equipes.</span><span class="sxs-lookup"><span data-stu-id="d53a0-140">List all groups that have teams.</span></span> |
|[<span data-ttu-id="d53a0-141">Publicar aplicativos para sua organização</span><span class="sxs-lookup"><span data-stu-id="d53a0-141">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="d53a0-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="d53a0-142">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="d53a0-143">Crie aplicativos do Teams que apenas sua organização possa ver.</span><span class="sxs-lookup"><span data-stu-id="d53a0-143">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="d53a0-144">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-144">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="d53a0-145">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d53a0-145">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="d53a0-146">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-146">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="d53a0-147">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="d53a0-147">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="d53a0-148">teamsTab</span><span class="sxs-lookup"><span data-stu-id="d53a0-148">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="d53a0-149">Adiciona (instala) uma guia no canal de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-149">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="d53a0-150">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d53a0-150">Properties</span></span>

| <span data-ttu-id="d53a0-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d53a0-151">Property</span></span> | <span data-ttu-id="d53a0-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="d53a0-152">Type</span></span>   | <span data-ttu-id="d53a0-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53a0-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d53a0-154">funSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-154">funSettings</span></span>|[<span data-ttu-id="d53a0-155">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-155">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="d53a0-156">Configurações que definem o uso de Giphy, memes e figurinhas na equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-156">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="d53a0-157">guestSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-157">guestSettings</span></span>|[<span data-ttu-id="d53a0-158">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-158">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="d53a0-159">Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-159">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="d53a0-160">internalId</span><span class="sxs-lookup"><span data-stu-id="d53a0-160">internalId</span></span> | <span data-ttu-id="d53a0-161">string</span><span class="sxs-lookup"><span data-stu-id="d53a0-161">string</span></span> | <span data-ttu-id="d53a0-162">Uma ID exclusiva da equipe, que foi usada em alguns locais, como o log de auditoria da [API da Atividade de Gestão do Office 365](/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="d53a0-162">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="d53a0-163">isArchived</span><span class="sxs-lookup"><span data-stu-id="d53a0-163">isArchived</span></span>|<span data-ttu-id="d53a0-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="d53a0-164">Boolean</span></span>|<span data-ttu-id="d53a0-165">Se essa equipe está no modo somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d53a0-165">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="d53a0-166">memberSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-166">memberSettings</span></span>|[<span data-ttu-id="d53a0-167">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-167">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="d53a0-168">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-168">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="d53a0-169">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-169">messagingSettings</span></span>|[<span data-ttu-id="d53a0-170">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-170">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="d53a0-171">Configurações para definir a mensagens e menções na equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-171">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="d53a0-172">webUrl</span><span class="sxs-lookup"><span data-stu-id="d53a0-172">webUrl</span></span>|<span data-ttu-id="d53a0-173">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="d53a0-173">string (readonly)</span></span> | <span data-ttu-id="d53a0-174">Um hiperlink que será enviado à equipe no cliente do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d53a0-174">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="d53a0-175">Esta é a URL que você recebe ao clicar com o botão direito do mouse em uma equipe no cliente do Microsoft Teams e escolher **Obter o link para a equipe**.</span><span class="sxs-lookup"><span data-stu-id="d53a0-175">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="d53a0-176">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="d53a0-176">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="d53a0-177">classSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-177">classSettings</span></span>|[<span data-ttu-id="d53a0-178">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="d53a0-178">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="d53a0-179">Definir configurações de uma classe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-179">Configure settings of a class.</span></span> <span data-ttu-id="d53a0-180">Disponível apenas quando a equipe representa uma classe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-180">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d53a0-181">Relações</span><span class="sxs-lookup"><span data-stu-id="d53a0-181">Relationships</span></span>

| <span data-ttu-id="d53a0-182">Relação</span><span class="sxs-lookup"><span data-stu-id="d53a0-182">Relationship</span></span> | <span data-ttu-id="d53a0-183">Tipo</span><span class="sxs-lookup"><span data-stu-id="d53a0-183">Type</span></span>   | <span data-ttu-id="d53a0-184">Descrição</span><span class="sxs-lookup"><span data-stu-id="d53a0-184">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d53a0-185">channels</span><span class="sxs-lookup"><span data-stu-id="d53a0-185">channels</span></span>|<span data-ttu-id="d53a0-186">Coleção [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="d53a0-186">[channel](channel.md) collection</span></span>|<span data-ttu-id="d53a0-187">A coleção de canais e mensagens associadas à equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-187">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="d53a0-188">installedApps</span><span class="sxs-lookup"><span data-stu-id="d53a0-188">installedApps</span></span>|<span data-ttu-id="d53a0-189">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="d53a0-189">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="d53a0-190">Os aplicativos instalados nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-190">The apps installed in this team.</span></span>|
|[<span data-ttu-id="d53a0-191">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="d53a0-191">primaryChannel</span></span>](../api/team-get-primarychannel.md)|[<span data-ttu-id="d53a0-192">channel</span><span class="sxs-lookup"><span data-stu-id="d53a0-192">channel</span></span>](channel.md)| <span data-ttu-id="d53a0-193">O canal geral da equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-193">The general channel for the team.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="d53a0-194">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d53a0-194">JSON representation</span></span>

<span data-ttu-id="d53a0-195">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d53a0-195">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="d53a0-196">**Observação:** se a equipe for do tipo classe, uma propriedade **classSettings** será aplicada à equipe.</span><span class="sxs-lookup"><span data-stu-id="d53a0-196">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
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

## <a name="see-also"></a><span data-ttu-id="d53a0-197">Confira também</span><span class="sxs-lookup"><span data-stu-id="d53a0-197">See Also</span></span>
- [<span data-ttu-id="d53a0-198">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="d53a0-198">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="d53a0-199">Como usar as APIs do Teams</span><span class="sxs-lookup"><span data-stu-id="d53a0-199">Using Teams APIs</span></span>](teams-api-overview.md)
