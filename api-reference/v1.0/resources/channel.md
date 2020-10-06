---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9860f6d1385374258eeed11dd8db4db21ba895c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364394"
---
# <a name="channel-resource-type"></a><span data-ttu-id="1a34d-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="1a34d-103">channel resource type</span></span>

<span data-ttu-id="1a34d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a34d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a34d-105">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="1a34d-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="1a34d-106">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="1a34d-106">Each channel is dedicated to a specific topic, department, or project.</span></span> <span data-ttu-id="1a34d-107">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="1a34d-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="1a34d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a34d-108">Methods</span></span>

| <span data-ttu-id="1a34d-109">Método</span><span class="sxs-lookup"><span data-stu-id="1a34d-109">Method</span></span>       | <span data-ttu-id="1a34d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a34d-110">Return Type</span></span>  |<span data-ttu-id="1a34d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a34d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a34d-112">List channels</span><span class="sxs-lookup"><span data-stu-id="1a34d-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="1a34d-113">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="1a34d-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="1a34d-114">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="1a34d-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="1a34d-115">Create channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="1a34d-116">channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-116">channel</span></span>](channel.md) | <span data-ttu-id="1a34d-117">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="1a34d-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="1a34d-118">Get channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="1a34d-119">channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-119">channel</span></span>](channel.md) | <span data-ttu-id="1a34d-120">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="1a34d-121">Update channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="1a34d-122">channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-122">channel</span></span>](channel.md) | <span data-ttu-id="1a34d-123">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="1a34d-124">Delete channel</span><span class="sxs-lookup"><span data-stu-id="1a34d-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="1a34d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a34d-125">None</span></span> | <span data-ttu-id="1a34d-126">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-126">Delete a channel.</span></span>|
|[<span data-ttu-id="1a34d-127">Listar guias</span><span class="sxs-lookup"><span data-stu-id="1a34d-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="1a34d-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1a34d-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1a34d-129">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-129">Lists tabs pinned to a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a34d-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a34d-130">Properties</span></span>

| <span data-ttu-id="1a34d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a34d-131">Property</span></span>   | <span data-ttu-id="1a34d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a34d-132">Type</span></span> |<span data-ttu-id="1a34d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a34d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a34d-134">description</span><span class="sxs-lookup"><span data-stu-id="1a34d-134">description</span></span>|<span data-ttu-id="1a34d-135">String</span><span class="sxs-lookup"><span data-stu-id="1a34d-135">String</span></span>|<span data-ttu-id="1a34d-136">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-136">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="1a34d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1a34d-137">displayName</span></span>|<span data-ttu-id="1a34d-138">String</span><span class="sxs-lookup"><span data-stu-id="1a34d-138">String</span></span>|<span data-ttu-id="1a34d-139">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a34d-139">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="1a34d-140">id</span><span class="sxs-lookup"><span data-stu-id="1a34d-140">id</span></span>|<span data-ttu-id="1a34d-141">String</span><span class="sxs-lookup"><span data-stu-id="1a34d-141">String</span></span>|<span data-ttu-id="1a34d-142">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-142">The channel's unique identifier.</span></span> <span data-ttu-id="1a34d-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a34d-143">Read-only.</span></span>|
|<span data-ttu-id="1a34d-144">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="1a34d-144">isFavoriteByDefault</span></span>|<span data-ttu-id="1a34d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a34d-145">Boolean</span></span>|<span data-ttu-id="1a34d-146">Indica se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="1a34d-146">Indicates whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="1a34d-147">Só pode ser definida por programação com [Criar equipe](../api/team-post.md).</span><span class="sxs-lookup"><span data-stu-id="1a34d-147">Can only be set programmatically with [Create team](../api/team-post.md).</span></span> <span data-ttu-id="1a34d-148">Padrão: `false`.</span><span class="sxs-lookup"><span data-stu-id="1a34d-148">Default: `false`.</span></span>|
|<span data-ttu-id="1a34d-149">email</span><span class="sxs-lookup"><span data-stu-id="1a34d-149">email</span></span>|<span data-ttu-id="1a34d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a34d-150">String</span></span>| <span data-ttu-id="1a34d-151">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-151">The email address for sending messages to the channel.</span></span> <span data-ttu-id="1a34d-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a34d-152">Read-only.</span></span>|
|<span data-ttu-id="1a34d-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="1a34d-153">webUrl</span></span>|<span data-ttu-id="1a34d-154">String</span><span class="sxs-lookup"><span data-stu-id="1a34d-154">String</span></span>|<span data-ttu-id="1a34d-155">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a34d-155">A hyperlink that will go to the channel in Microsoft Teams.</span></span> <span data-ttu-id="1a34d-156">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-156">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="1a34d-157">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="1a34d-157">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="1a34d-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a34d-158">Read-only.</span></span>|
|<span data-ttu-id="1a34d-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a34d-159">createdDateTime</span></span>|<span data-ttu-id="1a34d-160">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a34d-160">dateTimeOffset</span></span>|<span data-ttu-id="1a34d-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a34d-161">Read only.</span></span> <span data-ttu-id="1a34d-162">Carimbo de data/hora de criação do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-162">Timestamp at which the channel was created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a34d-163">Relações</span><span class="sxs-lookup"><span data-stu-id="1a34d-163">Relationships</span></span>

| <span data-ttu-id="1a34d-164">Relação</span><span class="sxs-lookup"><span data-stu-id="1a34d-164">Relationship</span></span> | <span data-ttu-id="1a34d-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a34d-165">Type</span></span> |<span data-ttu-id="1a34d-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a34d-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a34d-167">messages</span><span class="sxs-lookup"><span data-stu-id="1a34d-167">messages</span></span>|<span data-ttu-id="1a34d-168">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="1a34d-168">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="1a34d-169">Uma coleção de todas as mensagens do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-169">A collection of all the messages in the channel.</span></span> <span data-ttu-id="1a34d-170">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="1a34d-170">A navigation property.</span></span> <span data-ttu-id="1a34d-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1a34d-171">Nullable.</span></span>|
|<span data-ttu-id="1a34d-172">guias</span><span class="sxs-lookup"><span data-stu-id="1a34d-172">tabs</span></span>|<span data-ttu-id="1a34d-173">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="1a34d-173">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="1a34d-174">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="1a34d-174">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="1a34d-175">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="1a34d-175">A navigation property.</span></span>|
|[<span data-ttu-id="1a34d-176">filesFolder</span><span class="sxs-lookup"><span data-stu-id="1a34d-176">filesFolder</span></span>](../api/channel-get-filesfolder.md)|[<span data-ttu-id="1a34d-177">driveItem</span><span class="sxs-lookup"><span data-stu-id="1a34d-177">driveItem</span></span>](driveitem.md)|<span data-ttu-id="1a34d-178">Metadados para o local em que os arquivos do canal estão armazenados.</span><span class="sxs-lookup"><span data-stu-id="1a34d-178">Metadata for the location where the channel's files are stored.</span></span>|
|<span data-ttu-id="1a34d-179">operations</span><span class="sxs-lookup"><span data-stu-id="1a34d-179">operations</span></span>|<span data-ttu-id="1a34d-180">Coleção [teamsAsyncOperation](teamsasyncoperation.md)</span><span class="sxs-lookup"><span data-stu-id="1a34d-180">[teamsAsyncOperation](teamsasyncoperation.md) collection</span></span>| <span data-ttu-id="1a34d-181">As operações assíncronas que foram executadas ou estão em execução nesta equipe.</span><span class="sxs-lookup"><span data-stu-id="1a34d-181">The async operations that ran or are running on this team.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a34d-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a34d-182">JSON representation</span></span>

<span data-ttu-id="1a34d-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a34d-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "createdDateTime": "string (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
