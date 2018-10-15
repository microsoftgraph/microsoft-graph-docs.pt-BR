# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="dbb4d-101">Tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="dbb4d-101">patchContentCommand resource type</span></span>

<span data-ttu-id="dbb4d-102">As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-102">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbb4d-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbb4d-103">JSON representation</span></span>

<span data-ttu-id="dbb4d-104">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [PATCH pages/{id}\`](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="dbb4d-104">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page_update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="dbb4d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbb4d-105">Properties</span></span>
| <span data-ttu-id="dbb4d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbb4d-106">Property</span></span>     | <span data-ttu-id="dbb4d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb4d-107">Type</span></span>   |<span data-ttu-id="dbb4d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb4d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbb4d-109">action</span><span class="sxs-lookup"><span data-stu-id="dbb4d-109">action</span></span>|<span data-ttu-id="dbb4d-110">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="dbb4d-110">onenotePatchActionType values</span></span>|<span data-ttu-id="dbb4d-111">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-111">The action to perform on the target element.</span></span> <span data-ttu-id="dbb4d-112">Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-112">The possible values are `replace`, `append`, `delete`, `insert`, , , , , , , , or `prepend`.</span></span>|
|<span data-ttu-id="dbb4d-113">content</span><span class="sxs-lookup"><span data-stu-id="dbb4d-113">content</span></span>|<span data-ttu-id="dbb4d-114">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb4d-114">String</span></span>|<span data-ttu-id="dbb4d-p102">Uma cadeia de caracteres de HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="dbb4d-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="dbb4d-117">position</span><span class="sxs-lookup"><span data-stu-id="dbb4d-117">position</span></span>|<span data-ttu-id="dbb4d-118">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="dbb4d-118">onenotePatchInsertPosition values</span></span>|<span data-ttu-id="dbb4d-119">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-119">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="dbb4d-120">Os valores possíveis são: `after` (padrão) ou `before`.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-120">The possible values are , , , , , , , , , , , or .</span></span>|
|<span data-ttu-id="dbb4d-121">target</span><span class="sxs-lookup"><span data-stu-id="dbb4d-121">target</span></span>|<span data-ttu-id="dbb4d-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb4d-122">String</span></span>|<span data-ttu-id="dbb4d-p104">O elemento a atualizar. Deve ser o `#<data-id>` ou o `<id>` gerado do elemento ou a palavra-chave `body` ou `title`.</span><span class="sxs-lookup"><span data-stu-id="dbb4d-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
