# <a name="visualinfo-resource-type"></a><span data-ttu-id="232d2-101">tipo de recurso visualInfo</span><span class="sxs-lookup"><span data-stu-id="232d2-101">visualInfo resource type</span></span>

<span data-ttu-id="232d2-102">Um tipo complexo para representar a propriedade **visualElements** no objeto [activity](../resources/projectrome_activity.md).</span><span class="sxs-lookup"><span data-stu-id="232d2-102">A complex type for representing the **attribution** property in the [visualInfo part of the activity](../resources/projectrome_activity.md) object.</span></span>

<span data-ttu-id="232d2-103">Cada atividade do usuário será exibida na linha do tempo como um Cartão Adaptável.</span><span class="sxs-lookup"><span data-stu-id="232d2-103">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="232d2-104">Desenvolvedores de aplicativos são incentivados a fornecer um Cartão personalizado que captura a essência da atividade que foi realizada no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="232d2-104">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="232d2-105">É possível fazer isso fornecendo um cartão JSON personalizado na propriedade content.</span><span class="sxs-lookup"><span data-stu-id="232d2-105">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="232d2-106">Além de metadados visuais, com um Cartão Adaptável, o aplicativo pode especificar metadados de conteúdo – dados a serem usados para construir inferências sobre a atividade do usuário a fim de oferecer novas atividades para engajamento futuro.</span><span class="sxs-lookup"><span data-stu-id="232d2-106">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="232d2-107">Isso é possível usando a propriedade contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades de schema.org para descrever o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="232d2-107">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="232d2-108">Se não for fornecido um cartão personalizado, será gerado um cartão simples usando as propriedades displayText e description.</span><span class="sxs-lookup"><span data-stu-id="232d2-108">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="232d2-109">Cartões personalizados são recomendados para demonstrar o melhor conteúdo do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="232d2-109">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="232d2-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="232d2-110">Properties</span></span>

|<span data-ttu-id="232d2-111">Nome</span><span class="sxs-lookup"><span data-stu-id="232d2-111">Name</span></span> | <span data-ttu-id="232d2-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="232d2-112">Type</span></span> | <span data-ttu-id="232d2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="232d2-113">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="232d2-114">displayText</span><span class="sxs-lookup"><span data-stu-id="232d2-114">displayText</span></span> | <span data-ttu-id="232d2-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="232d2-115">String</span></span> | <span data-ttu-id="232d2-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="232d2-116">Required.</span></span> <span data-ttu-id="232d2-117">Uma breve descrição em texto sobre a atividade exclusiva do usuário (por exemplo, nome do documento em casos onde uma atividade refere-se à criação de documentos)</span><span class="sxs-lookup"><span data-stu-id="232d2-117">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="232d2-118">descrição</span><span class="sxs-lookup"><span data-stu-id="232d2-118">description</span></span> | <span data-ttu-id="232d2-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="232d2-119">String</span></span> | <span data-ttu-id="232d2-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="232d2-120">Optional.</span></span> <span data-ttu-id="232d2-121">Descrição de texto mais longa da atividade exclusiva do usuário (exemplo: nome, primeira frase e/ou metadados de documentos)</span><span class="sxs-lookup"><span data-stu-id="232d2-121">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="232d2-122">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="232d2-122">background-color</span></span> | <span data-ttu-id="232d2-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="232d2-123">String</span></span> | <span data-ttu-id="232d2-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="232d2-124">Optional.</span></span> <span data-ttu-id="232d2-125">Cor do plano de fundo usada para processar a atividade na interface do usuário - cor de marca para a fonte da atividade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="232d2-125">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="232d2-126">Deve ser uma cor hexadecimal válida</span><span class="sxs-lookup"><span data-stu-id="232d2-126">Must be a valid hex color</span></span>|
|<span data-ttu-id="232d2-127">content</span><span class="sxs-lookup"><span data-stu-id="232d2-127">content</span></span> | <span data-ttu-id="232d2-128">Objeto JSON não tipado</span><span class="sxs-lookup"><span data-stu-id="232d2-128">Untyped JSON object</span></span> | <span data-ttu-id="232d2-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="232d2-129">Optional.</span></span> <span data-ttu-id="232d2-130">Parte personalizada de dados - objeto JSON usado para fornecer conteúdo personalizado para renderizar a atividade na interface de usuário do Shell do Windows</span><span class="sxs-lookup"><span data-stu-id="232d2-130">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="232d2-131">attribution</span><span class="sxs-lookup"><span data-stu-id="232d2-131">attribution</span></span> | <span data-ttu-id="232d2-132">[imageInfo](../resources/projectrome_imageinfo.md)</span><span class="sxs-lookup"><span data-stu-id="232d2-132">Added [imageInfo](../resources/projectrome_imageinfo.md)</span></span> | <span data-ttu-id="232d2-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="232d2-133">Optional.</span></span> <span data-ttu-id="232d2-134">Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="232d2-134">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="232d2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="232d2-135">JSON Representation</span></span>

<span data-ttu-id="232d2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="232d2-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
