---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1db6133b4bb4c74e9515a9f14cc6f430ef0e32d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033010"
---
# <a name="channel-resource-type"></a><span data-ttu-id="89c5e-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="89c5e-103">channel resource type</span></span>

<span data-ttu-id="89c5e-104">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="89c5e-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="89c5e-105">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="89c5e-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="89c5e-106">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="89c5e-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="89c5e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="89c5e-107">Methods</span></span>

| <span data-ttu-id="89c5e-108">Método</span><span class="sxs-lookup"><span data-stu-id="89c5e-108">Method</span></span>       | <span data-ttu-id="89c5e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89c5e-109">Return Type</span></span>  |<span data-ttu-id="89c5e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="89c5e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89c5e-111">List channels</span><span class="sxs-lookup"><span data-stu-id="89c5e-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="89c5e-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="89c5e-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="89c5e-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="89c5e-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="89c5e-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="89c5e-115">channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-115">channel</span></span>](channel.md) | <span data-ttu-id="89c5e-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="89c5e-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="89c5e-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="89c5e-118">channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-118">channel</span></span>](channel.md) | <span data-ttu-id="89c5e-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="89c5e-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="89c5e-121">channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-121">channel</span></span>](channel.md) | <span data-ttu-id="89c5e-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="89c5e-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="89c5e-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="89c5e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89c5e-124">None</span></span> | <span data-ttu-id="89c5e-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-125">Delete a channel.</span></span>|
|[<span data-ttu-id="89c5e-126">Listar guias</span><span class="sxs-lookup"><span data-stu-id="89c5e-126">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="89c5e-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="89c5e-127">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="89c5e-128">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-128">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="89c5e-129">Obter guia</span><span class="sxs-lookup"><span data-stu-id="89c5e-129">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="89c5e-130">teamsTab</span><span class="sxs-lookup"><span data-stu-id="89c5e-130">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="89c5e-131">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-131">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="89c5e-132">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="89c5e-132">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="89c5e-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="89c5e-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="89c5e-134">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-134">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="89c5e-135">Remover guia</span><span class="sxs-lookup"><span data-stu-id="89c5e-135">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="89c5e-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89c5e-136">None</span></span> | <span data-ttu-id="89c5e-137">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-137">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="89c5e-138">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="89c5e-138">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="89c5e-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="89c5e-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="89c5e-140">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="89c5e-140">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="89c5e-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89c5e-141">Properties</span></span>
| <span data-ttu-id="89c5e-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89c5e-142">Property</span></span>     | <span data-ttu-id="89c5e-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="89c5e-143">Type</span></span>   |<span data-ttu-id="89c5e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="89c5e-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89c5e-145">description</span><span class="sxs-lookup"><span data-stu-id="89c5e-145">description</span></span>|<span data-ttu-id="89c5e-146">String</span><span class="sxs-lookup"><span data-stu-id="89c5e-146">String</span></span>|<span data-ttu-id="89c5e-147">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-147">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="89c5e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="89c5e-148">displayName</span></span>|<span data-ttu-id="89c5e-149">String</span><span class="sxs-lookup"><span data-stu-id="89c5e-149">String</span></span>|<span data-ttu-id="89c5e-150">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="89c5e-150">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="89c5e-151">email</span><span class="sxs-lookup"><span data-stu-id="89c5e-151">email</span></span>|<span data-ttu-id="89c5e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89c5e-152">String</span></span>| <span data-ttu-id="89c5e-153">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-153">The email address for sending messages to the channel.</span></span> <span data-ttu-id="89c5e-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89c5e-154">Read-only.</span></span>|
|<span data-ttu-id="89c5e-155">id</span><span class="sxs-lookup"><span data-stu-id="89c5e-155">id</span></span>|<span data-ttu-id="89c5e-156">String</span><span class="sxs-lookup"><span data-stu-id="89c5e-156">String</span></span>|<span data-ttu-id="89c5e-157">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-157">The channels's unique identifier.</span></span> <span data-ttu-id="89c5e-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89c5e-158">Read-only.</span></span>|
|<span data-ttu-id="89c5e-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="89c5e-159">webUrl</span></span>|<span data-ttu-id="89c5e-160">String</span><span class="sxs-lookup"><span data-stu-id="89c5e-160">String</span></span>|<span data-ttu-id="89c5e-161">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="89c5e-161">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="89c5e-162">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-162">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="89c5e-163">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="89c5e-163">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="89c5e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89c5e-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89c5e-165">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="89c5e-165">Relationships</span></span>
| <span data-ttu-id="89c5e-166">Relação</span><span class="sxs-lookup"><span data-stu-id="89c5e-166">Relationship</span></span> | <span data-ttu-id="89c5e-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="89c5e-167">Type</span></span>   |<span data-ttu-id="89c5e-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="89c5e-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89c5e-169">guias</span><span class="sxs-lookup"><span data-stu-id="89c5e-169">tabs</span></span>|<span data-ttu-id="89c5e-170">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="89c5e-170">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="89c5e-171">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="89c5e-171">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="89c5e-172">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="89c5e-172">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="89c5e-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89c5e-173">JSON representation</span></span>

<span data-ttu-id="89c5e-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="89c5e-174">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
