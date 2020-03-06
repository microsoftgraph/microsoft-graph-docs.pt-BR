---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4117190df40eb3bcf5a837fdad298cefe5121793
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531933"
---
# <a name="channel-resource-type"></a><span data-ttu-id="eb93c-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="eb93c-103">channel resource type</span></span>

<span data-ttu-id="eb93c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb93c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb93c-105">[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas.</span><span class="sxs-lookup"><span data-stu-id="eb93c-105">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="eb93c-106">Cada canal é dedicado a um tópico específico, departamento ou projeto.</span><span class="sxs-lookup"><span data-stu-id="eb93c-106">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="eb93c-107">Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.</span><span class="sxs-lookup"><span data-stu-id="eb93c-107">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="eb93c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb93c-108">Methods</span></span>

| <span data-ttu-id="eb93c-109">Método</span><span class="sxs-lookup"><span data-stu-id="eb93c-109">Method</span></span>       | <span data-ttu-id="eb93c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb93c-110">Return Type</span></span>  |<span data-ttu-id="eb93c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb93c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb93c-112">List channels</span><span class="sxs-lookup"><span data-stu-id="eb93c-112">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="eb93c-113">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="eb93c-113">[channel](channel.md) collection</span></span> | <span data-ttu-id="eb93c-114">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="eb93c-114">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="eb93c-115">Create channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-115">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="eb93c-116">channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-116">channel</span></span>](channel.md) | <span data-ttu-id="eb93c-117">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="eb93c-117">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="eb93c-118">Get channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-118">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="eb93c-119">channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-119">channel</span></span>](channel.md) | <span data-ttu-id="eb93c-120">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-120">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="eb93c-121">Update channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-121">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="eb93c-122">channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-122">channel</span></span>](channel.md) | <span data-ttu-id="eb93c-123">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-123">Update properties of the channel.</span></span>|
|[<span data-ttu-id="eb93c-124">Delete channel</span><span class="sxs-lookup"><span data-stu-id="eb93c-124">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="eb93c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb93c-125">None</span></span> | <span data-ttu-id="eb93c-126">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-126">Delete a channel.</span></span>|
|[<span data-ttu-id="eb93c-127">Listar guias</span><span class="sxs-lookup"><span data-stu-id="eb93c-127">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="eb93c-128">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eb93c-128">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eb93c-129">Listar guias fixadas a um canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-129">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="eb93c-130">Obter guia</span><span class="sxs-lookup"><span data-stu-id="eb93c-130">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="eb93c-131">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eb93c-131">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eb93c-132">Ler uma guia fixada a um canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-132">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="eb93c-133">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="eb93c-133">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="eb93c-134">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eb93c-134">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eb93c-135">Adicionar (fixar) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-135">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="eb93c-136">Remover guia</span><span class="sxs-lookup"><span data-stu-id="eb93c-136">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="eb93c-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb93c-137">None</span></span> | <span data-ttu-id="eb93c-138">Remover (desafixar) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-138">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="eb93c-139">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="eb93c-139">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="eb93c-140">teamsTab</span><span class="sxs-lookup"><span data-stu-id="eb93c-140">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="eb93c-141">Atualizar as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="eb93c-141">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb93c-142">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb93c-142">Properties</span></span>
| <span data-ttu-id="eb93c-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb93c-143">Property</span></span>     | <span data-ttu-id="eb93c-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb93c-144">Type</span></span>   |<span data-ttu-id="eb93c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb93c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb93c-146">description</span><span class="sxs-lookup"><span data-stu-id="eb93c-146">description</span></span>|<span data-ttu-id="eb93c-147">String</span><span class="sxs-lookup"><span data-stu-id="eb93c-147">String</span></span>|<span data-ttu-id="eb93c-148">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-148">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="eb93c-149">displayName</span><span class="sxs-lookup"><span data-stu-id="eb93c-149">displayName</span></span>|<span data-ttu-id="eb93c-150">String</span><span class="sxs-lookup"><span data-stu-id="eb93c-150">String</span></span>|<span data-ttu-id="eb93c-151">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eb93c-151">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="eb93c-152">email</span><span class="sxs-lookup"><span data-stu-id="eb93c-152">email</span></span>|<span data-ttu-id="eb93c-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb93c-153">String</span></span>| <span data-ttu-id="eb93c-154">O endereço de email para enviar mensagens ao canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-154">The email address for sending messages to the channel.</span></span> <span data-ttu-id="eb93c-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb93c-155">Read-only.</span></span>|
|<span data-ttu-id="eb93c-156">id</span><span class="sxs-lookup"><span data-stu-id="eb93c-156">id</span></span>|<span data-ttu-id="eb93c-157">String</span><span class="sxs-lookup"><span data-stu-id="eb93c-157">String</span></span>|<span data-ttu-id="eb93c-158">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-158">The channels's unique identifier.</span></span> <span data-ttu-id="eb93c-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb93c-159">Read-only.</span></span>|
|<span data-ttu-id="eb93c-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="eb93c-160">webUrl</span></span>|<span data-ttu-id="eb93c-161">String</span><span class="sxs-lookup"><span data-stu-id="eb93c-161">String</span></span>|<span data-ttu-id="eb93c-162">Um hiperlink que navegará até o canal no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eb93c-162">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="eb93c-163">Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-163">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="eb93c-164">Essa URL deve ser tratada como um blob opaco e não analisado.</span><span class="sxs-lookup"><span data-stu-id="eb93c-164">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="eb93c-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb93c-165">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb93c-166">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="eb93c-166">Relationships</span></span>
| <span data-ttu-id="eb93c-167">Relação</span><span class="sxs-lookup"><span data-stu-id="eb93c-167">Relationship</span></span> | <span data-ttu-id="eb93c-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb93c-168">Type</span></span>   |<span data-ttu-id="eb93c-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb93c-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb93c-170">guias</span><span class="sxs-lookup"><span data-stu-id="eb93c-170">tabs</span></span>|<span data-ttu-id="eb93c-171">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="eb93c-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="eb93c-172">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="eb93c-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="eb93c-173">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="eb93c-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb93c-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb93c-174">JSON representation</span></span>

<span data-ttu-id="eb93c-175">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="eb93c-175">Here is a JSON representation of the resource</span></span>

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
