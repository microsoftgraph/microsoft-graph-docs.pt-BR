# <a name="extensionschemaproperty-resource-type"></a><span data-ttu-id="4542a-101">Tipo de recurso extensionSchemaProperty</span><span class="sxs-lookup"><span data-stu-id="4542a-101">extensionSchemaProperty resource type</span></span>

<span data-ttu-id="4542a-102">Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="4542a-102">Use the **extensionSchemaProperty** resource to define a property's name and its type, as part of a [schemaExtension](schemaextension.md) definition.</span></span>


## <a name="properties"></a><span data-ttu-id="4542a-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4542a-103">Properties</span></span>
| <span data-ttu-id="4542a-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4542a-104">Property</span></span>     | <span data-ttu-id="4542a-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="4542a-105">Type</span></span>   |<span data-ttu-id="4542a-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="4542a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4542a-107">name</span><span class="sxs-lookup"><span data-stu-id="4542a-107">name</span></span>|<span data-ttu-id="4542a-108">String</span><span class="sxs-lookup"><span data-stu-id="4542a-108">String</span></span>| <span data-ttu-id="4542a-109">O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="4542a-109">The name of the strongly-typed property defined as part of a schema extension.</span></span>|
|<span data-ttu-id="4542a-110">type</span><span class="sxs-lookup"><span data-stu-id="4542a-110">type</span></span>|<span data-ttu-id="4542a-111">String</span><span class="sxs-lookup"><span data-stu-id="4542a-111">String</span></span>| <span data-ttu-id="4542a-p101">O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="4542a-p101">The type of the property that is defined as part of a schema extension.  Allowed values are *Binary, Boolean, DateTime, Integer* or *String*.  See the table below for more details.</span></span>|

#### <a name="supported-property-data-types"></a><span data-ttu-id="4542a-115">Tipos de dados de propriedade com suporte</span><span class="sxs-lookup"><span data-stu-id="4542a-115">Supported property data types</span></span> 
<span data-ttu-id="4542a-116">Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:</span><span class="sxs-lookup"><span data-stu-id="4542a-116">The following data types are supported when defining a property in a schema extension:</span></span>

| <span data-ttu-id="4542a-117">Tipo de propriedade</span><span class="sxs-lookup"><span data-stu-id="4542a-117">Property Type</span></span> | <span data-ttu-id="4542a-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="4542a-118">Remarks</span></span> |
|-------------|------------|
| <span data-ttu-id="4542a-119">Binária</span><span class="sxs-lookup"><span data-stu-id="4542a-119">Binary</span></span> | <span data-ttu-id="4542a-120">No máximo 256 bytes.</span><span class="sxs-lookup"><span data-stu-id="4542a-120">256 bytes maximum.</span></span> |
| <span data-ttu-id="4542a-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="4542a-121">Boolean</span></span> | <span data-ttu-id="4542a-122">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="4542a-122">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="4542a-123">DateTime</span><span class="sxs-lookup"><span data-stu-id="4542a-123">DateTime</span></span> | <span data-ttu-id="4542a-p102">Deve ser especificado no formato ISO 8601. Serão armazenados no UTC.</span><span class="sxs-lookup"><span data-stu-id="4542a-p102">Must be specified in ISO 8601 format. Will be stored in UTC.</span></span> |
| <span data-ttu-id="4542a-126">Número inteiro</span><span class="sxs-lookup"><span data-stu-id="4542a-126">Integer</span></span> | <span data-ttu-id="4542a-127">Valor de 32 bits.</span><span class="sxs-lookup"><span data-stu-id="4542a-127">32-bit value.</span></span> <span data-ttu-id="4542a-128">Não é compatível com os contatos, mensagens, eventos e postagens.</span><span class="sxs-lookup"><span data-stu-id="4542a-128">Not supported for messages, events and posts.</span></span> |
| <span data-ttu-id="4542a-129">String</span><span class="sxs-lookup"><span data-stu-id="4542a-129">String</span></span> | <span data-ttu-id="4542a-130">Máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4542a-130">256 characters maximum.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4542a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4542a-131">JSON representation</span></span>
<span data-ttu-id="4542a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4542a-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
