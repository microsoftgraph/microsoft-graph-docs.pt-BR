# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="9c7b9-101">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9c7b9-101">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="9c7b9-102">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-102">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="9c7b9-103">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="9c7b9-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c7b9-104">Methods</span></span>

| <span data-ttu-id="9c7b9-105">Método</span><span class="sxs-lookup"><span data-stu-id="9c7b9-105">Method</span></span>           | <span data-ttu-id="9c7b9-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c7b9-106">Return Type</span></span>    |<span data-ttu-id="9c7b9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c7b9-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c7b9-108">Postar</span><span class="sxs-lookup"><span data-stu-id="9c7b9-108">Post</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | <span data-ttu-id="9c7b9-p101">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="9c7b9-111">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-111">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="9c7b9-112">Obter</span><span class="sxs-lookup"><span data-stu-id="9c7b9-112">Get</span></span>](../api/multivaluelegacyextendedproperty_get.md) |<span data-ttu-id="9c7b9-113">Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="9c7b9-113">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="9c7b9-114">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-114">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c7b9-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c7b9-115">Properties</span></span>
| <span data-ttu-id="9c7b9-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c7b9-116">Property</span></span>     | <span data-ttu-id="9c7b9-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c7b9-117">Type</span></span>   |<span data-ttu-id="9c7b9-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c7b9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c7b9-119">id</span><span class="sxs-lookup"><span data-stu-id="9c7b9-119">id</span></span>|<span data-ttu-id="9c7b9-120">string</span><span class="sxs-lookup"><span data-stu-id="9c7b9-120">string</span></span>|<span data-ttu-id="9c7b9-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="9c7b9-123">valor</span><span class="sxs-lookup"><span data-stu-id="9c7b9-123">value</span></span>|<span data-ttu-id="9c7b9-124">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c7b9-124">string collection</span></span>|<span data-ttu-id="9c7b9-125">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-125">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c7b9-126">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9c7b9-126">Relationships</span></span>
<span data-ttu-id="9c7b9-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c7b9-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9c7b9-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c7b9-128">JSON representation</span></span>

<span data-ttu-id="9c7b9-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c7b9-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->