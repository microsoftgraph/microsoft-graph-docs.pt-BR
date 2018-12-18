---
title: tipo de recurso de canal
description: 'Um canal é uma coleção de mensagens dentro de uma equipe. '
author: nkramer
ms.openlocfilehash: f9ab71213180732a0c8c626d5b32b9074bd135d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337083"
---
# <a name="channel-resource-type"></a><span data-ttu-id="94284-103">tipo de recurso de canal</span><span class="sxs-lookup"><span data-stu-id="94284-103">channel resource type</span></span>



<span data-ttu-id="94284-104">Um canal é uma coleção de mensagens dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="94284-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="94284-105">Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="94284-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="94284-106">Exemplos podem ser canal "Sexta-feira equipe almoço" e "Discussão sobre a arquitetura" channel.</span><span class="sxs-lookup"><span data-stu-id="94284-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="94284-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="94284-107">Methods</span></span>

| <span data-ttu-id="94284-108">Método</span><span class="sxs-lookup"><span data-stu-id="94284-108">Method</span></span>       | <span data-ttu-id="94284-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="94284-109">Return Type</span></span>  |<span data-ttu-id="94284-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94284-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94284-111">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="94284-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="94284-112">coleção de [canal](channel.md)</span><span class="sxs-lookup"><span data-stu-id="94284-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="94284-113">Obter a lista de canais nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="94284-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="94284-114">Criar canal</span><span class="sxs-lookup"><span data-stu-id="94284-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="94284-115">canal</span><span class="sxs-lookup"><span data-stu-id="94284-115">channel</span></span>](channel.md) | <span data-ttu-id="94284-116">Crie um novo canal, incluindo o nome para exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="94284-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="94284-117">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="94284-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="94284-118">canal</span><span class="sxs-lookup"><span data-stu-id="94284-118">channel</span></span>](channel.md) | <span data-ttu-id="94284-119">Leia as propriedades e os relacionamentos do canal.</span><span class="sxs-lookup"><span data-stu-id="94284-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="94284-120">Canal de atualização</span><span class="sxs-lookup"><span data-stu-id="94284-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="94284-121">canal</span><span class="sxs-lookup"><span data-stu-id="94284-121">channel</span></span>](channel.md) | <span data-ttu-id="94284-122">Atualize propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="94284-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="94284-123">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="94284-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="94284-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94284-124">None</span></span> | <span data-ttu-id="94284-125">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="94284-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="94284-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94284-126">Properties</span></span>
| <span data-ttu-id="94284-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94284-127">Property</span></span>     | <span data-ttu-id="94284-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="94284-128">Type</span></span>   |<span data-ttu-id="94284-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="94284-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94284-130">description</span><span class="sxs-lookup"><span data-stu-id="94284-130">description</span></span>|<span data-ttu-id="94284-131">String</span><span class="sxs-lookup"><span data-stu-id="94284-131">String</span></span>|<span data-ttu-id="94284-132">Descrição textual opcional para o canal.</span><span class="sxs-lookup"><span data-stu-id="94284-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="94284-133">displayName</span><span class="sxs-lookup"><span data-stu-id="94284-133">displayName</span></span>|<span data-ttu-id="94284-134">String</span><span class="sxs-lookup"><span data-stu-id="94284-134">String</span></span>|<span data-ttu-id="94284-135">Nome de canal como ele será exibido ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="94284-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="94284-136">id</span><span class="sxs-lookup"><span data-stu-id="94284-136">id</span></span>|<span data-ttu-id="94284-137">String</span><span class="sxs-lookup"><span data-stu-id="94284-137">String</span></span>|<span data-ttu-id="94284-138">Identificador exclusivo dos canais.</span><span class="sxs-lookup"><span data-stu-id="94284-138">The channels's unique identifier.</span></span> <span data-ttu-id="94284-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94284-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94284-140">Relações</span><span class="sxs-lookup"><span data-stu-id="94284-140">Relationships</span></span>
| <span data-ttu-id="94284-141">Relação</span><span class="sxs-lookup"><span data-stu-id="94284-141">Relationship</span></span> | <span data-ttu-id="94284-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="94284-142">Type</span></span>   |<span data-ttu-id="94284-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="94284-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94284-144">guias</span><span class="sxs-lookup"><span data-stu-id="94284-144">tabs</span></span>|<span data-ttu-id="94284-145">coleção [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="94284-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="94284-146">Uma coleção de todas as guias no canal.</span><span class="sxs-lookup"><span data-stu-id="94284-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="94284-147">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="94284-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="94284-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94284-148">JSON representation</span></span>

<span data-ttu-id="94284-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="94284-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
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
