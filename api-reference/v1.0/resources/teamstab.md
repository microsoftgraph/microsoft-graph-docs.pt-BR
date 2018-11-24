# <a name="teamstab-resource-type"></a><span data-ttu-id="1407a-101">tipo de recurso de teamsTab</span><span class="sxs-lookup"><span data-stu-id="1407a-101">teamsTab resource type</span></span>



<span data-ttu-id="1407a-102">Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="1407a-102">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="1407a-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="1407a-103">Methods</span></span>

| <span data-ttu-id="1407a-104">Método</span><span class="sxs-lookup"><span data-stu-id="1407a-104">Method</span></span>       | <span data-ttu-id="1407a-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1407a-105">Return Type</span></span>  |<span data-ttu-id="1407a-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="1407a-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1407a-107">Guias de lista</span><span class="sxs-lookup"><span data-stu-id="1407a-107">List tabs</span></span>](../api/teamstab_list.md) | [<span data-ttu-id="1407a-108">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1407a-108">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1407a-109">Guias de listas fixados em um canal.</span><span class="sxs-lookup"><span data-stu-id="1407a-109">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="1407a-110">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="1407a-110">Get tab</span></span>](../api/teamstab_get.md) | [<span data-ttu-id="1407a-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1407a-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1407a-112">Lê uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="1407a-112">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="1407a-113">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="1407a-113">Add tab</span></span>](../api/teamstab_add.md) | [<span data-ttu-id="1407a-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1407a-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1407a-115">Adiciona (pins) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="1407a-115">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="1407a-116">Remover guia</span><span class="sxs-lookup"><span data-stu-id="1407a-116">Remove tab</span></span>](../api/teamstab_delete.md) | <span data-ttu-id="1407a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1407a-117">None</span></span> | <span data-ttu-id="1407a-118">Remove (unpin) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="1407a-118">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="1407a-119">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="1407a-119">Update tab</span></span>](../api/teamstab_update.md) | [<span data-ttu-id="1407a-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="1407a-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="1407a-121">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="1407a-121">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="1407a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1407a-122">Properties</span></span>

|<span data-ttu-id="1407a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1407a-123">Property</span></span>|<span data-ttu-id="1407a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1407a-124">Type</span></span>|<span data-ttu-id="1407a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1407a-125">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="1407a-126">id</span><span class="sxs-lookup"><span data-stu-id="1407a-126">id</span></span>              |   <span data-ttu-id="1407a-127">string</span><span class="sxs-lookup"><span data-stu-id="1407a-127">string</span></span>                  |  <span data-ttu-id="1407a-128">Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.</span><span class="sxs-lookup"><span data-stu-id="1407a-128">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="1407a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1407a-129">displayName</span></span>            |   <span data-ttu-id="1407a-130">string</span><span class="sxs-lookup"><span data-stu-id="1407a-130">string</span></span>                  |  <span data-ttu-id="1407a-131">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="1407a-131">Name of the tab.</span></span>     |
|  <span data-ttu-id="1407a-132">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="1407a-132">sortOrderIndex</span></span>  |   <span data-ttu-id="1407a-133">inteiro</span><span class="sxs-lookup"><span data-stu-id="1407a-133">int</span></span>                     |  <span data-ttu-id="1407a-134">Índice da ordem usada para classificar as guias</span><span class="sxs-lookup"><span data-stu-id="1407a-134">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="1407a-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="1407a-135">webUrl</span></span>          |   <span data-ttu-id="1407a-136">string</span><span class="sxs-lookup"><span data-stu-id="1407a-136">string</span></span>                  |  <span data-ttu-id="1407a-137">Link profundo url da instância do guia.</span><span class="sxs-lookup"><span data-stu-id="1407a-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="1407a-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1407a-138">Read only.</span></span>     |
|  <span data-ttu-id="1407a-139">configuration</span><span class="sxs-lookup"><span data-stu-id="1407a-139">configuration</span></span>        |   [<span data-ttu-id="1407a-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="1407a-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="1407a-141">Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="1407a-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="1407a-142">Relações</span><span class="sxs-lookup"><span data-stu-id="1407a-142">Relationships</span></span>

| <span data-ttu-id="1407a-143">Relação</span><span class="sxs-lookup"><span data-stu-id="1407a-143">Relationship</span></span> | <span data-ttu-id="1407a-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="1407a-144">Type</span></span>   | <span data-ttu-id="1407a-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="1407a-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1407a-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1407a-146">teamsApp</span></span>|[<span data-ttu-id="1407a-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="1407a-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="1407a-148">O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da guia.</span><span class="sxs-lookup"><span data-stu-id="1407a-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1407a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1407a-149">JSON representation</span></span>

<span data-ttu-id="1407a-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1407a-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="1407a-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="1407a-151">See also</span></span>

[<span data-ttu-id="1407a-152">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="1407a-152">Configuring the built-in tab types</span></span>](../../../concepts/teams-configuring-builtin-tabs.md)
