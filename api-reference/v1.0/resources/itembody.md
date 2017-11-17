# <a name="itembody-resource-type"></a><span data-ttu-id="a51d8-101">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="a51d8-101">itemBody resource type</span></span>

<span data-ttu-id="a51d8-102">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="a51d8-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="a51d8-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a51d8-103">Properties</span></span>
| <span data-ttu-id="a51d8-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a51d8-104">Property</span></span>     | <span data-ttu-id="a51d8-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="a51d8-105">Type</span></span>   |<span data-ttu-id="a51d8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="a51d8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a51d8-107">content</span><span class="sxs-lookup"><span data-stu-id="a51d8-107">content</span></span>|<span data-ttu-id="a51d8-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a51d8-108">String</span></span>|<span data-ttu-id="a51d8-109">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="a51d8-109">The content of the item.</span></span>|
|<span data-ttu-id="a51d8-110">contentType</span><span class="sxs-lookup"><span data-stu-id="a51d8-110">contentType</span></span>|<span data-ttu-id="a51d8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a51d8-111">String</span></span>|<span data-ttu-id="a51d8-p101">O tipo de conteúdo. Os valores possíveis são: `Text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="a51d8-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a51d8-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a51d8-114">JSON representation</span></span>

<span data-ttu-id="a51d8-115">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a51d8-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
