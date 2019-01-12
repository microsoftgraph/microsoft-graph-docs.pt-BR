---
title: tipo de recurso de visualInfo
description: Um tipo complexo para representar a propriedade **visualElements** no objeto de atividade.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 416109bb1bb6625330ddfbbb32b8fb688b223134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962643"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="a4bca-103">tipo de recurso de visualInfo</span><span class="sxs-lookup"><span data-stu-id="a4bca-103">visualInfo resource type</span></span>

<span data-ttu-id="a4bca-104">Um tipo complexo para representar a propriedade **visualElements** no objeto de [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="a4bca-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="a4bca-105">Cada atividade do usuário será exibida na linha do tempo como um cartão adaptável.</span><span class="sxs-lookup"><span data-stu-id="a4bca-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="a4bca-106">Desenvolvedores de aplicativos são incentivados a fornecer um cartão personalizado que captura a essência da atividade que foi realizada no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4bca-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="a4bca-107">Isso é possível, fornecendo um cartão JSON personalizado na propriedade conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a4bca-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="a4bca-108">Além dos metadados visual com uma placa adaptável, app pode especificar metadados do conteúdo – dados a ser usado para construir Inferências sobre a atividade do usuário a fim de oferecer novas atividades para o compromisso re futura.</span><span class="sxs-lookup"><span data-stu-id="a4bca-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="a4bca-109">Isso é possível usando a propriedade de contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades de schema.org para descrever o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a4bca-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="a4bca-110">Se não for fornecido um cartão personalizado, será gerado um cartão simple usando propriedades displayText e descrição.</span><span class="sxs-lookup"><span data-stu-id="a4bca-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="a4bca-111">Cartões personalizados são recomendados para demonstrar o melhor conteúdo de dentro de seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4bca-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="a4bca-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4bca-112">Properties</span></span>

|<span data-ttu-id="a4bca-113">Nome</span><span class="sxs-lookup"><span data-stu-id="a4bca-113">Name</span></span> | <span data-ttu-id="a4bca-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4bca-114">Type</span></span> | <span data-ttu-id="a4bca-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4bca-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="a4bca-116">displayText</span><span class="sxs-lookup"><span data-stu-id="a4bca-116">displayText</span></span> | <span data-ttu-id="a4bca-117">String</span><span class="sxs-lookup"><span data-stu-id="a4bca-117">String</span></span> | <span data-ttu-id="a4bca-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4bca-118">Required.</span></span> <span data-ttu-id="a4bca-119">Uma breve descrição de texto de atividade de exclusivo do usuário (por exemplo, nome do documento em casos onde uma atividade refere-se a criação de documentos)</span><span class="sxs-lookup"><span data-stu-id="a4bca-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="a4bca-120">description</span><span class="sxs-lookup"><span data-stu-id="a4bca-120">description</span></span> | <span data-ttu-id="a4bca-121">String</span><span class="sxs-lookup"><span data-stu-id="a4bca-121">String</span></span> | <span data-ttu-id="a4bca-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4bca-122">Optional.</span></span> <span data-ttu-id="a4bca-123">Descrição de texto mais longa da atividade exclusivo do usuário (exemplo: nome, primeira frase e/ou metadados de documentos)</span><span class="sxs-lookup"><span data-stu-id="a4bca-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="a4bca-124">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="a4bca-124">backgroundColor</span></span> | <span data-ttu-id="a4bca-125">String</span><span class="sxs-lookup"><span data-stu-id="a4bca-125">String</span></span> | <span data-ttu-id="a4bca-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4bca-126">Optional.</span></span> <span data-ttu-id="a4bca-127">Cor de plano de fundo usada para processar a atividade na interface do usuário - cor de marca para a fonte da atividade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4bca-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="a4bca-128">Deve ser uma cor hexadecimal válida</span><span class="sxs-lookup"><span data-stu-id="a4bca-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="a4bca-129">content</span><span class="sxs-lookup"><span data-stu-id="a4bca-129">content</span></span> | <span data-ttu-id="a4bca-130">Objeto sem JSON</span><span class="sxs-lookup"><span data-stu-id="a4bca-130">Untyped JSON object</span></span> | <span data-ttu-id="a4bca-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4bca-131">Optional.</span></span> <span data-ttu-id="a4bca-132">Parte personalizada de dados - objeto JSON usados para fornecer conteúdo personalizado para renderizar a atividade no UI do Shell do Windows</span><span class="sxs-lookup"><span data-stu-id="a4bca-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="a4bca-133">attribution</span><span class="sxs-lookup"><span data-stu-id="a4bca-133">attribution</span></span> | [<span data-ttu-id="a4bca-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="a4bca-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="a4bca-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a4bca-135">Optional.</span></span> <span data-ttu-id="a4bca-136">Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="a4bca-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4bca-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4bca-137">JSON Representation</span></span>

<span data-ttu-id="a4bca-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4bca-138">The following is a JSON representation of the resource.</span></span>

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
