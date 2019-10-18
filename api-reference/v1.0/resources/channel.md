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
# <a name="channel-resource-type"></a><span data-ttu-id="bac2d-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="bac2d-103">channel resource type</span></span>

<span data-ttu-id="bac2d-104">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="bac2d-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="bac2d-105">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="bac2d-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="bac2d-106">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="bac2d-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="bac2d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bac2d-107">Methods</span></span>

| <span data-ttu-id="bac2d-108">Método</span><span class="sxs-lookup"><span data-stu-id="bac2d-108">Method</span></span>       | <span data-ttu-id="bac2d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bac2d-109">Return Type</span></span>  |<span data-ttu-id="bac2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac2d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bac2d-111">List channels</span><span class="sxs-lookup"><span data-stu-id="bac2d-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="bac2d-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="bac2d-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="bac2d-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="bac2d-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="bac2d-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="bac2d-115">channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-115">channel</span></span>](channel.md) | <span data-ttu-id="bac2d-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="bac2d-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="bac2d-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="bac2d-118">channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-118">channel</span></span>](channel.md) | <span data-ttu-id="bac2d-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="bac2d-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="bac2d-121">channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-121">channel</span></span>](channel.md) | <span data-ttu-id="bac2d-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="bac2d-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="bac2d-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="bac2d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bac2d-124">None</span></span> | <span data-ttu-id="bac2d-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-125">Delete a channel.</span></span>|
|[<span data-ttu-id="bac2d-126">Listar guias</span><span class="sxs-lookup"><span data-stu-id="bac2d-126">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="bac2d-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bac2d-127">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bac2d-128">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-128">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="bac2d-129">Obter guia</span><span class="sxs-lookup"><span data-stu-id="bac2d-129">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="bac2d-130">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bac2d-130">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bac2d-131">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-131">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="bac2d-132">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="bac2d-132">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="bac2d-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bac2d-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bac2d-134">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-134">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="bac2d-135">Remover guia</span><span class="sxs-lookup"><span data-stu-id="bac2d-135">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="bac2d-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bac2d-136">None</span></span> | <span data-ttu-id="bac2d-137">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-137">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="bac2d-138">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="bac2d-138">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="bac2d-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bac2d-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bac2d-140">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="bac2d-140">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="bac2d-141">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bac2d-141">Properties</span></span>
| <span data-ttu-id="bac2d-142">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bac2d-142">Property</span></span>     | <span data-ttu-id="bac2d-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="bac2d-143">Type</span></span>   |<span data-ttu-id="bac2d-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac2d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bac2d-145">description</span><span class="sxs-lookup"><span data-stu-id="bac2d-145">description</span></span>|<span data-ttu-id="bac2d-146">String</span><span class="sxs-lookup"><span data-stu-id="bac2d-146">String</span></span>|<span data-ttu-id="bac2d-147">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-147">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="bac2d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="bac2d-148">displayName</span></span>|<span data-ttu-id="bac2d-149">String</span><span class="sxs-lookup"><span data-stu-id="bac2d-149">String</span></span>|<span data-ttu-id="bac2d-150">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bac2d-150">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="bac2d-151">email</span><span class="sxs-lookup"><span data-stu-id="bac2d-151">email</span></span>|<span data-ttu-id="bac2d-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bac2d-152">String</span></span>| <span data-ttu-id="bac2d-153">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-153">The email address for sending messages to the channel.</span></span> <span data-ttu-id="bac2d-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bac2d-154">Read-only.</span></span>|
|<span data-ttu-id="bac2d-155">id</span><span class="sxs-lookup"><span data-stu-id="bac2d-155">id</span></span>|<span data-ttu-id="bac2d-156">String</span><span class="sxs-lookup"><span data-stu-id="bac2d-156">String</span></span>|<span data-ttu-id="bac2d-157">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-157">The channels's unique identifier.</span></span> <span data-ttu-id="bac2d-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bac2d-158">Read-only.</span></span>|
|<span data-ttu-id="bac2d-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="bac2d-159">webUrl</span></span>|<span data-ttu-id="bac2d-160">String</span><span class="sxs-lookup"><span data-stu-id="bac2d-160">String</span></span>|<span data-ttu-id="bac2d-161">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bac2d-161">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="bac2d-162">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-162">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="bac2d-163">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="bac2d-163">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="bac2d-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bac2d-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac2d-165">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="bac2d-165">Relationships</span></span>
| <span data-ttu-id="bac2d-166">Relação</span><span class="sxs-lookup"><span data-stu-id="bac2d-166">Relationship</span></span> | <span data-ttu-id="bac2d-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="bac2d-167">Type</span></span>   |<span data-ttu-id="bac2d-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac2d-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bac2d-169">guias</span><span class="sxs-lookup"><span data-stu-id="bac2d-169">tabs</span></span>|<span data-ttu-id="bac2d-170">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="bac2d-170">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="bac2d-171">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="bac2d-171">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="bac2d-172">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="bac2d-172">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bac2d-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bac2d-173">JSON representation</span></span>

<span data-ttu-id="bac2d-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bac2d-174">Here is a JSON representation of the resource</span></span>

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
