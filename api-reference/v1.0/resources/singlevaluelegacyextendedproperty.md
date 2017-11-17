# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="9aad1-101">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9aad1-101">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="9aad1-102">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="9aad1-102">An extended property that contains a single value.</span></span> 

<span data-ttu-id="9aad1-103">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="9aad1-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="9aad1-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="9aad1-104">Methods</span></span>

| <span data-ttu-id="9aad1-105">Método</span><span class="sxs-lookup"><span data-stu-id="9aad1-105">Method</span></span>           | <span data-ttu-id="9aad1-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9aad1-106">Return Type</span></span>    |<span data-ttu-id="9aad1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aad1-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9aad1-108">Post</span><span class="sxs-lookup"><span data-stu-id="9aad1-108">Post</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | <span data-ttu-id="9aad1-109">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md), mas não o grupo [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="9aad1-109">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="9aad1-110">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="9aad1-110">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="9aad1-111">Get</span><span class="sxs-lookup"><span data-stu-id="9aad1-111">Get</span></span>](../api/singlevaluelegacyextendedproperty_get.md) |<span data-ttu-id="9aad1-112">Uma ou mais instâncias de recurso compatíveis ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="9aad1-112">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="9aad1-113">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9aad1-113">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="9aad1-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aad1-114">Properties</span></span>
| <span data-ttu-id="9aad1-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aad1-115">Property</span></span>     | <span data-ttu-id="9aad1-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aad1-116">Type</span></span>   |<span data-ttu-id="9aad1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aad1-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9aad1-118">id</span><span class="sxs-lookup"><span data-stu-id="9aad1-118">id</span></span>|<span data-ttu-id="9aad1-119">string</span><span class="sxs-lookup"><span data-stu-id="9aad1-119">string</span></span>|<span data-ttu-id="9aad1-p101">A ID da propriedade usada para identificar a propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9aad1-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="9aad1-122">value</span><span class="sxs-lookup"><span data-stu-id="9aad1-122">value</span></span>|<span data-ttu-id="9aad1-123">string</span><span class="sxs-lookup"><span data-stu-id="9aad1-123">string</span></span>|<span data-ttu-id="9aad1-124">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9aad1-124">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aad1-125">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9aad1-125">Relationships</span></span>
<span data-ttu-id="9aad1-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9aad1-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9aad1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aad1-127">JSON representation</span></span>

<span data-ttu-id="9aad1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9aad1-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->