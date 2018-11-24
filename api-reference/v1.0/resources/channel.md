# <a name="channel-resource-type"></a><span data-ttu-id="e7c1a-101">tipo de recurso de canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-101">channel resource type</span></span>



<span data-ttu-id="e7c1a-102">Um canal é uma coleção de mensagens dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="e7c1a-102">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="e7c1a-103">Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-103">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="e7c1a-104">Exemplos podem ser canal "Sexta-feira equipe almoço" e "Discussão sobre a arquitetura" channel.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-104">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="e7c1a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e7c1a-105">Methods</span></span>

| <span data-ttu-id="e7c1a-106">Método</span><span class="sxs-lookup"><span data-stu-id="e7c1a-106">Method</span></span>       | <span data-ttu-id="e7c1a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7c1a-107">Return Type</span></span>  |<span data-ttu-id="e7c1a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7c1a-109">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="e7c1a-109">List channels</span></span>](../api/channel_list.md) | <span data-ttu-id="e7c1a-110">coleção de [canal](channel.md)</span><span class="sxs-lookup"><span data-stu-id="e7c1a-110">[channel](channel.md) collection</span></span> | <span data-ttu-id="e7c1a-111">Obter a lista de canais nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-111">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="e7c1a-112">Criar canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-112">Create channel</span></span>](../api/channel_post.md) | [<span data-ttu-id="e7c1a-113">canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-113">channel</span></span>](channel.md) | <span data-ttu-id="e7c1a-114">Crie um novo canal, incluindo o nome para exibição e a descrição.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-114">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="e7c1a-115">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-115">Get channel</span></span>](../api/channel_get.md) | [<span data-ttu-id="e7c1a-116">canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-116">channel</span></span>](channel.md) | <span data-ttu-id="e7c1a-117">Leia as propriedades e os relacionamentos do canal.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-117">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="e7c1a-118">Canal de atualização</span><span class="sxs-lookup"><span data-stu-id="e7c1a-118">Update channel</span></span>](../api/channel_patch.md) | [<span data-ttu-id="e7c1a-119">canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-119">channel</span></span>](channel.md) | <span data-ttu-id="e7c1a-120">Atualize propriedades do canal.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-120">Update properties of the channel.</span></span>|
|[<span data-ttu-id="e7c1a-121">Excluir um canal</span><span class="sxs-lookup"><span data-stu-id="e7c1a-121">Delete channel</span></span>](../api/channel_delete.md) | <span data-ttu-id="e7c1a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7c1a-122">None</span></span> | <span data-ttu-id="e7c1a-123">Exclua um canal.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-123">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7c1a-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7c1a-124">Properties</span></span>
| <span data-ttu-id="e7c1a-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7c1a-125">Property</span></span>     | <span data-ttu-id="e7c1a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7c1a-126">Type</span></span>   |<span data-ttu-id="e7c1a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c1a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7c1a-128">description</span><span class="sxs-lookup"><span data-stu-id="e7c1a-128">description</span></span>|<span data-ttu-id="e7c1a-129">String</span><span class="sxs-lookup"><span data-stu-id="e7c1a-129">String</span></span>|<span data-ttu-id="e7c1a-130">Descrição textual opcional para o canal.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-130">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="e7c1a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e7c1a-131">displayName</span></span>|<span data-ttu-id="e7c1a-132">String</span><span class="sxs-lookup"><span data-stu-id="e7c1a-132">String</span></span>|<span data-ttu-id="e7c1a-133">Nome de canal como ele será exibido ao usuário no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-133">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e7c1a-134">id</span><span class="sxs-lookup"><span data-stu-id="e7c1a-134">id</span></span>|<span data-ttu-id="e7c1a-135">String</span><span class="sxs-lookup"><span data-stu-id="e7c1a-135">String</span></span>|<span data-ttu-id="e7c1a-136">Identificador exclusivo dos canais.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-136">The channels's unique identifier.</span></span> <span data-ttu-id="e7c1a-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7c1a-138">Relações</span><span class="sxs-lookup"><span data-stu-id="e7c1a-138">Relationships</span></span>
| <span data-ttu-id="e7c1a-139">Relação</span><span class="sxs-lookup"><span data-stu-id="e7c1a-139">Relationship</span></span> | <span data-ttu-id="e7c1a-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7c1a-140">Type</span></span>   |<span data-ttu-id="e7c1a-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c1a-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7c1a-142">guias</span><span class="sxs-lookup"><span data-stu-id="e7c1a-142">tabs</span></span>|<span data-ttu-id="e7c1a-143">coleção [teamsTab](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="e7c1a-143">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="e7c1a-144">Uma coleção de todas as guias no canal.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-144">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="e7c1a-145">Uma propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="e7c1a-145">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e7c1a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7c1a-146">JSON representation</span></span>

<span data-ttu-id="e7c1a-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e7c1a-147">Here is a JSON representation of the resource</span></span>

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
