# <a name="imageinfo-resource-type"></a><span data-ttu-id="d1eb8-101">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="d1eb8-101">imageInfo resource type</span></span>

<span data-ttu-id="d1eb8-102">Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome_visualinfo.md) do objeto [atividade](../resources/projectrome_activity.md).</span><span class="sxs-lookup"><span data-stu-id="d1eb8-102">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome_visualinfo.md) part of the [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="d1eb8-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1eb8-103">Properties</span></span>

|<span data-ttu-id="d1eb8-104">Nome</span><span class="sxs-lookup"><span data-stu-id="d1eb8-104">Name</span></span> | <span data-ttu-id="d1eb8-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1eb8-105">Type</span></span> | <span data-ttu-id="d1eb8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1eb8-106">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d1eb8-107">iconurl</span><span class="sxs-lookup"><span data-stu-id="d1eb8-107">iconurl</span></span> | <span data-ttu-id="d1eb8-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1eb8-108">String</span></span> | <span data-ttu-id="d1eb8-109">Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="d1eb8-109">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="d1eb8-110">alternateText</span><span class="sxs-lookup"><span data-stu-id="d1eb8-110">alternateText</span></span> | <span data-ttu-id="d1eb8-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1eb8-111">String</span></span> | <span data-ttu-id="d1eb8-112">Opcional; conteúdo de texto ALT acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="d1eb8-112">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="d1eb8-113">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="d1eb8-113">addImageQuery</span></span> | <span data-ttu-id="d1eb8-114">Booleano</span><span class="sxs-lookup"><span data-stu-id="d1eb8-114">Boolean</span></span> | <span data-ttu-id="d1eb8-115">Opcional; parâmetro usado para indicar que o servidor é capaz de processar imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="d1eb8-115">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="d1eb8-116">Por exemplo, – uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="d1eb8-116">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1eb8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1eb8-117">JSON Representation</span></span>

<span data-ttu-id="d1eb8-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d1eb8-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->