---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 052c6d8fc298e929dfd1c69e1b64debb7e14eb4a
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994451"
---
# <a name="channel-resource-type"></a><span data-ttu-id="e6df2-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="e6df2-103">channel resource type</span></span>



<span data-ttu-id="e6df2-104">Um canal é um conjunto de mensagens em um [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="e6df2-104">A channel is a collection of chatMessages within a team.</span></span> <span data-ttu-id="e6df2-105">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="e6df2-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="e6df2-106">Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .</span><span class="sxs-lookup"><span data-stu-id="e6df2-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="e6df2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6df2-107">Methods</span></span>

| <span data-ttu-id="e6df2-108">Método</span><span class="sxs-lookup"><span data-stu-id="e6df2-108">Method</span></span>       | <span data-ttu-id="e6df2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6df2-109">Return Type</span></span>  |<span data-ttu-id="e6df2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6df2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6df2-111">List channels</span><span class="sxs-lookup"><span data-stu-id="e6df2-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="e6df2-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="e6df2-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="e6df2-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="e6df2-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="e6df2-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="e6df2-115">channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-115">channel</span></span>](channel.md) | <span data-ttu-id="e6df2-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="e6df2-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="e6df2-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="e6df2-118">channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-118">channel</span></span>](channel.md) | <span data-ttu-id="e6df2-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="e6df2-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="e6df2-121">channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-121">channel</span></span>](channel.md) | <span data-ttu-id="e6df2-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="e6df2-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="e6df2-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="e6df2-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6df2-124">None</span></span> | <span data-ttu-id="e6df2-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6df2-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6df2-126">Properties</span></span>
| <span data-ttu-id="e6df2-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6df2-127">Property</span></span>     | <span data-ttu-id="e6df2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6df2-128">Type</span></span>   |<span data-ttu-id="e6df2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6df2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6df2-130">description</span><span class="sxs-lookup"><span data-stu-id="e6df2-130">description</span></span>|<span data-ttu-id="e6df2-131">String</span><span class="sxs-lookup"><span data-stu-id="e6df2-131">String</span></span>|<span data-ttu-id="e6df2-132">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="e6df2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e6df2-133">displayName</span></span>|<span data-ttu-id="e6df2-134">String</span><span class="sxs-lookup"><span data-stu-id="e6df2-134">String</span></span>|<span data-ttu-id="e6df2-135">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e6df2-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e6df2-136">id</span><span class="sxs-lookup"><span data-stu-id="e6df2-136">id</span></span>|<span data-ttu-id="e6df2-137">String</span><span class="sxs-lookup"><span data-stu-id="e6df2-137">String</span></span>|<span data-ttu-id="e6df2-138">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-138">The channels's unique identifier.</span></span> <span data-ttu-id="e6df2-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6df2-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6df2-140">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="e6df2-140">Relationships</span></span>
| <span data-ttu-id="e6df2-141">Relação</span><span class="sxs-lookup"><span data-stu-id="e6df2-141">Relationship</span></span> | <span data-ttu-id="e6df2-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6df2-142">Type</span></span>   |<span data-ttu-id="e6df2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6df2-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6df2-144">guias</span><span class="sxs-lookup"><span data-stu-id="e6df2-144">tabs</span></span>|<span data-ttu-id="e6df2-145">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="e6df2-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="e6df2-146">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="e6df2-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="e6df2-147">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="e6df2-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e6df2-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6df2-148">JSON representation</span></span>

<span data-ttu-id="e6df2-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e6df2-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
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
