---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163711"
---
# <a name="channel-resource-type"></a><span data-ttu-id="273b5-103">Tipo de recurso de usuário</span><span class="sxs-lookup"><span data-stu-id="273b5-103">channel resource type</span></span>



<span data-ttu-id="273b5-104">Um canal é um conjunto de mensagens em um [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="273b5-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="273b5-105">Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="273b5-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="273b5-106">Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .</span><span class="sxs-lookup"><span data-stu-id="273b5-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="273b5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="273b5-107">Methods</span></span>

| <span data-ttu-id="273b5-108">Método</span><span class="sxs-lookup"><span data-stu-id="273b5-108">Method</span></span>       | <span data-ttu-id="273b5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="273b5-109">Return Type</span></span>  |<span data-ttu-id="273b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="273b5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="273b5-111">List channels</span><span class="sxs-lookup"><span data-stu-id="273b5-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="273b5-112">[channel](channel.md) collection</span><span class="sxs-lookup"><span data-stu-id="273b5-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="273b5-113">Obtenha a lista de canais nessa equipe.</span><span class="sxs-lookup"><span data-stu-id="273b5-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="273b5-114">Create channel</span><span class="sxs-lookup"><span data-stu-id="273b5-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="273b5-115">channel</span><span class="sxs-lookup"><span data-stu-id="273b5-115">channel</span></span>](channel.md) | <span data-ttu-id="273b5-116">Crie um novo canal ao incluir o nome de exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="273b5-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="273b5-117">Get channel</span><span class="sxs-lookup"><span data-stu-id="273b5-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="273b5-118">channel</span><span class="sxs-lookup"><span data-stu-id="273b5-118">channel</span></span>](channel.md) | <span data-ttu-id="273b5-119">Leia as propriedades e as relações do canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="273b5-120">Update channel</span><span class="sxs-lookup"><span data-stu-id="273b5-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="273b5-121">channel</span><span class="sxs-lookup"><span data-stu-id="273b5-121">channel</span></span>](channel.md) | <span data-ttu-id="273b5-122">Atualize as propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="273b5-123">Delete channel</span><span class="sxs-lookup"><span data-stu-id="273b5-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="273b5-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="273b5-124">None</span></span> | <span data-ttu-id="273b5-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="273b5-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="273b5-126">Properties</span></span>
| <span data-ttu-id="273b5-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="273b5-127">Property</span></span>     | <span data-ttu-id="273b5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="273b5-128">Type</span></span>   |<span data-ttu-id="273b5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="273b5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="273b5-130">description</span><span class="sxs-lookup"><span data-stu-id="273b5-130">description</span></span>|<span data-ttu-id="273b5-131">String</span><span class="sxs-lookup"><span data-stu-id="273b5-131">String</span></span>|<span data-ttu-id="273b5-132">Descrição textual opcional do canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="273b5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="273b5-133">displayName</span></span>|<span data-ttu-id="273b5-134">String</span><span class="sxs-lookup"><span data-stu-id="273b5-134">String</span></span>|<span data-ttu-id="273b5-135">Nome do canal como ele aparecerá ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="273b5-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="273b5-136">id</span><span class="sxs-lookup"><span data-stu-id="273b5-136">id</span></span>|<span data-ttu-id="273b5-137">String</span><span class="sxs-lookup"><span data-stu-id="273b5-137">String</span></span>|<span data-ttu-id="273b5-138">O identificador exclusivo do canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-138">The channels's unique identifier.</span></span> <span data-ttu-id="273b5-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="273b5-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="273b5-140">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="273b5-140">Relationships</span></span>
| <span data-ttu-id="273b5-141">Relação</span><span class="sxs-lookup"><span data-stu-id="273b5-141">Relationship</span></span> | <span data-ttu-id="273b5-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="273b5-142">Type</span></span>   |<span data-ttu-id="273b5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="273b5-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="273b5-144">guias</span><span class="sxs-lookup"><span data-stu-id="273b5-144">tabs</span></span>|<span data-ttu-id="273b5-145">[teamsTab](../resources/teamstab.md) collection</span><span class="sxs-lookup"><span data-stu-id="273b5-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="273b5-146">Uma coleção de todas as guias do canal.</span><span class="sxs-lookup"><span data-stu-id="273b5-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="273b5-147">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="273b5-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="273b5-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="273b5-148">JSON representation</span></span>

<span data-ttu-id="273b5-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="273b5-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
