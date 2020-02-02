---
title: tipo de recurso de equipe
description: 'No Microsoft Teams, uma equipe é um conjunto de canais. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3f221f91de856cc2816e309923c48926624b8e63
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652155"
---
# <a name="team-resource-type"></a><span data-ttu-id="532f2-103">tipo de recurso de equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-103">team resource type</span></span>



<span data-ttu-id="532f2-104">No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md).</span><span class="sxs-lookup"><span data-stu-id="532f2-104">A team in Microsoft Teams is a collection of [channel](channel.md) objects.</span></span>
<span data-ttu-id="532f2-105">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span>

<span data-ttu-id="532f2-106">Cada equipe está associada a um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="532f2-106">Every team is associated with a [group](../resources/group.md).</span></span>
<span data-ttu-id="532f2-107">O grupo tem a mesma ID da equipe, por exemplo, /groups/{id}/team é igual a /teams/{id}.</span><span class="sxs-lookup"><span data-stu-id="532f2-107">The group has the same ID as the team - for example, /groups/{id}/team is the same as /teams/{id}.</span></span>
<span data-ttu-id="532f2-108">Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).</span><span class="sxs-lookup"><span data-stu-id="532f2-108">For more information about working with groups and members in teams, see [Use the Microsoft Graph REST API to work with Microsoft Teams](teams-api-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="532f2-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="532f2-109">Methods</span></span>

| <span data-ttu-id="532f2-110">Método</span><span class="sxs-lookup"><span data-stu-id="532f2-110">Method</span></span>       | <span data-ttu-id="532f2-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="532f2-111">Return Type</span></span>  |<span data-ttu-id="532f2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="532f2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="532f2-113">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-113">Create team</span></span>](../api/team-put-teams.md) | [<span data-ttu-id="532f2-114">team</span><span class="sxs-lookup"><span data-stu-id="532f2-114">team</span></span>](team.md) | <span data-ttu-id="532f2-115">Crie uma nova equipe ou adicione uma equipe a um grupo existente.</span><span class="sxs-lookup"><span data-stu-id="532f2-115">Create a new team, or add a team to an existing group.</span></span>|
|[<span data-ttu-id="532f2-116">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-116">Get team</span></span>](../api/team-get.md) | [<span data-ttu-id="532f2-117">team</span><span class="sxs-lookup"><span data-stu-id="532f2-117">team</span></span>](team.md) | <span data-ttu-id="532f2-118">Recupere as propriedades e relações da equipe especificada.</span><span class="sxs-lookup"><span data-stu-id="532f2-118">Retrieve the properties and relationships of the specified team.</span></span>|
|[<span data-ttu-id="532f2-119">Atualizar equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-119">Update team</span></span>](../api/team-update.md) | [<span data-ttu-id="532f2-120">team</span><span class="sxs-lookup"><span data-stu-id="532f2-120">team</span></span>](team.md) |<span data-ttu-id="532f2-121">Atualize as propriedades da equipe especificada.</span><span class="sxs-lookup"><span data-stu-id="532f2-121">Update the properties of the specified team.</span></span> |
|[<span data-ttu-id="532f2-122">Excluir equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-122">Delete team</span></span>](/graph/api/group-delete?view=graph-rest-1.0) | <span data-ttu-id="532f2-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="532f2-123">None</span></span> |<span data-ttu-id="532f2-124">Exclua a equipe e o grupo associado.</span><span class="sxs-lookup"><span data-stu-id="532f2-124">Delete the team and its associated group.</span></span> |
|[<span data-ttu-id="532f2-125">Clonar equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-125">Clone team</span></span>](../api/team-clone.md) | [<span data-ttu-id="532f2-126">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="532f2-126">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="532f2-127">Copie a equipe e o grupo associado.</span><span class="sxs-lookup"><span data-stu-id="532f2-127">Copy the team and its associated group.</span></span> |
|[<span data-ttu-id="532f2-128">Arquivar equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-128">Archive team</span></span>](../api/team-archive.md) | [<span data-ttu-id="532f2-129">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="532f2-129">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="532f2-130">Coloque a equipe em um estado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="532f2-130">Put the team in a read-only state.</span></span> |
|[<span data-ttu-id="532f2-131">Desarquivar equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-131">Unarchive team</span></span>](../api/team-unarchive.md) | [<span data-ttu-id="532f2-132">teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="532f2-132">teamsAsyncOperation</span></span>](../resources/teamsasyncoperation.md) |<span data-ttu-id="532f2-133">Restaure a equipe com um estado de leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="532f2-133">Restore the team to a read-write state.</span></span> |
|[<span data-ttu-id="532f2-134">Listar suas equipes</span><span class="sxs-lookup"><span data-stu-id="532f2-134">List your teams</span></span>](../api/user-list-joinedteams.md) | <span data-ttu-id="532f2-135">Coleção [team](team.md)</span><span class="sxs-lookup"><span data-stu-id="532f2-135">[team](team.md) collection</span></span> | <span data-ttu-id="532f2-136">Liste as equipes das quais você é membro.</span><span class="sxs-lookup"><span data-stu-id="532f2-136">List the teams you are a member of.</span></span> |
|[<span data-ttu-id="532f2-137">Listar todas as equipes</span><span class="sxs-lookup"><span data-stu-id="532f2-137">List all teams</span></span>](/graph/teams-list-all-teams) | <span data-ttu-id="532f2-138">Coleção [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="532f2-138">[group](group.md) collection</span></span> | <span data-ttu-id="532f2-139">Liste todos os grupos que têm equipes.</span><span class="sxs-lookup"><span data-stu-id="532f2-139">List all groups that have teams.</span></span> |
|[<span data-ttu-id="532f2-140">Publicar aplicativos para sua organização</span><span class="sxs-lookup"><span data-stu-id="532f2-140">Publish apps to your organization</span></span>](../resources/teamsapp.md)| [<span data-ttu-id="532f2-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="532f2-141">teamsApp</span></span>](../resources/teamsapp.md) | <span data-ttu-id="532f2-142">Crie aplicativos do Teams que apenas sua organização possa ver.</span><span class="sxs-lookup"><span data-stu-id="532f2-142">Create Teams apps visible only to your organization.</span></span> |
|[<span data-ttu-id="532f2-143">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-143">Add app to team</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="532f2-144">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="532f2-144">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="532f2-145">Adiciona (instala) um aplicativo a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-145">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="532f2-146">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="532f2-146">Add tab to channel</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="532f2-147">teamsTab</span><span class="sxs-lookup"><span data-stu-id="532f2-147">teamsTab</span></span>](../resources/teamstab.md) | <span data-ttu-id="532f2-148">Adiciona (instala) uma guia no canal de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-148">Adds (installs) a tab to a team's channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="532f2-149">Propriedades</span><span class="sxs-lookup"><span data-stu-id="532f2-149">Properties</span></span>

| <span data-ttu-id="532f2-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="532f2-150">Property</span></span> | <span data-ttu-id="532f2-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="532f2-151">Type</span></span>   | <span data-ttu-id="532f2-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="532f2-152">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="532f2-153">funSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-153">funSettings</span></span>|[<span data-ttu-id="532f2-154">teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-154">teamFunSettings</span></span>](teamfunsettings.md) |<span data-ttu-id="532f2-155">Configurações que definem o uso de Giphy, memes e figurinhas na equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-155">Settings to configure use of Giphy, memes, and stickers in the team.</span></span>|
|<span data-ttu-id="532f2-156">guestSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-156">guestSettings</span></span>|[<span data-ttu-id="532f2-157">teamGuestSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-157">teamGuestSettings</span></span>](teamguestsettings.md) |<span data-ttu-id="532f2-158">Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-158">Settings to configure whether guests can create, update, or delete channels in the team.</span></span>|
|<span data-ttu-id="532f2-159">internalId</span><span class="sxs-lookup"><span data-stu-id="532f2-159">internalId</span></span> | <span data-ttu-id="532f2-160">string</span><span class="sxs-lookup"><span data-stu-id="532f2-160">string</span></span> | <span data-ttu-id="532f2-161">Uma ID exclusiva da equipe, que foi usada em alguns locais, como o log de auditoria da [API da Atividade de Gestão do Office 365](/office/office-365-management-api/office-365-management-activity-api-reference).</span><span class="sxs-lookup"><span data-stu-id="532f2-161">A unique ID for the team that has been used in a few places such as the audit log/[Office 365 Management Activity API](/office/office-365-management-api/office-365-management-activity-api-reference).</span></span> |
|<span data-ttu-id="532f2-162">isArchived</span><span class="sxs-lookup"><span data-stu-id="532f2-162">isArchived</span></span>|<span data-ttu-id="532f2-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="532f2-163">Boolean</span></span>|<span data-ttu-id="532f2-164">Se essa equipe está no modo somente leitura.</span><span class="sxs-lookup"><span data-stu-id="532f2-164">Whether this team is in read-only mode.</span></span> |
|<span data-ttu-id="532f2-165">memberSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-165">memberSettings</span></span>|[<span data-ttu-id="532f2-166">teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-166">teamMemberSettings</span></span>](teammembersettings.md) |<span data-ttu-id="532f2-167">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-167">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the team.</span></span>|
|<span data-ttu-id="532f2-168">messagingSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-168">messagingSettings</span></span>|[<span data-ttu-id="532f2-169">teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-169">teamMessagingSettings</span></span>](teammessagingsettings.md) |<span data-ttu-id="532f2-170">Configurações para definir a mensagens e menções na equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-170">Settings to configure messaging and mentions in the team.</span></span>|
|<span data-ttu-id="532f2-171">webUrl</span><span class="sxs-lookup"><span data-stu-id="532f2-171">webUrl</span></span>|<span data-ttu-id="532f2-172">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="532f2-172">string (readonly)</span></span> | <span data-ttu-id="532f2-173">Um hiperlink que será enviado à equipe no cliente do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="532f2-173">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="532f2-174">Esta é a URL que você recebe ao clicar com o botão direito do mouse em uma equipe no cliente do Microsoft Teams e escolher **Obter o link para a equipe**.</span><span class="sxs-lookup"><span data-stu-id="532f2-174">This is the URL that you get when you right-click a team in the Microsoft Teams client and select **Get link to team**.</span></span> <span data-ttu-id="532f2-175">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="532f2-175">This URL should be treated as an opaque blob, and not parsed.</span></span> |
|<span data-ttu-id="532f2-176">classSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-176">classSettings</span></span>|[<span data-ttu-id="532f2-177">teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="532f2-177">teamClassSettings</span></span>](teamclasssettings.md) |<span data-ttu-id="532f2-178">Definir configurações de uma classe.</span><span class="sxs-lookup"><span data-stu-id="532f2-178">Configure settings of a class.</span></span> <span data-ttu-id="532f2-179">Disponível apenas quando a equipe representa uma classe.</span><span class="sxs-lookup"><span data-stu-id="532f2-179">Available only when the team represents a class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="532f2-180">Relações</span><span class="sxs-lookup"><span data-stu-id="532f2-180">Relationships</span></span>

| <span data-ttu-id="532f2-181">Relação</span><span class="sxs-lookup"><span data-stu-id="532f2-181">Relationship</span></span> | <span data-ttu-id="532f2-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="532f2-182">Type</span></span>   | <span data-ttu-id="532f2-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="532f2-183">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="532f2-184">channels</span><span class="sxs-lookup"><span data-stu-id="532f2-184">channels</span></span>|<span data-ttu-id="532f2-185">Coleção [channel](channel.md)</span><span class="sxs-lookup"><span data-stu-id="532f2-185">[channel](channel.md) collection</span></span>|<span data-ttu-id="532f2-186">A coleção de canais e mensagens associadas à equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-186">The collection of channels & messages associated with the team.</span></span>|
|<span data-ttu-id="532f2-187">installedApps</span><span class="sxs-lookup"><span data-stu-id="532f2-187">installedApps</span></span>|<span data-ttu-id="532f2-188">Coleção [teamsAppInstallation](teamsappinstallation.md)</span><span class="sxs-lookup"><span data-stu-id="532f2-188">[teamsAppInstallation](teamsappinstallation.md) collection</span></span>|<span data-ttu-id="532f2-189">Os aplicativos instalados nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-189">The apps installed in this team.</span></span>|
|<span data-ttu-id="532f2-190">primaryChannel</span><span class="sxs-lookup"><span data-stu-id="532f2-190">primaryChannel</span></span>|[<span data-ttu-id="532f2-191">canal</span><span class="sxs-lookup"><span data-stu-id="532f2-191">channel</span></span>](channel.md)| <span data-ttu-id="532f2-192">O canal geral da equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-192">The general channel for the team.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="532f2-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="532f2-193">JSON representation</span></span>

<span data-ttu-id="532f2-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="532f2-194">The following is a JSON representation of the resource.</span></span>

><span data-ttu-id="532f2-195">**Observação:** se a equipe for do tipo classe, uma propriedade **classSettings** será aplicada à equipe.</span><span class="sxs-lookup"><span data-stu-id="532f2-195">**Note:** If the team is of type class, a **classSettings** property is applied on the team.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="532f2-196">Confira também</span><span class="sxs-lookup"><span data-stu-id="532f2-196">See Also</span></span>
- [<span data-ttu-id="532f2-197">Como criar um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="532f2-197">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
- [<span data-ttu-id="532f2-198">Como usar as APIs do Teams</span><span class="sxs-lookup"><span data-stu-id="532f2-198">Using Teams APIs</span></span>](teams-api-overview.md)
