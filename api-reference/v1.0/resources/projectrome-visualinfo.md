---
title: tipo de recurso visualInfo
description: Um tipo complexo para representar a propriedade **visualElements** no objeto Activity.
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e97e7d295d9a228d44adf355b510adb90a0b3f96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447042"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="5c816-103">tipo de recurso visualInfo</span><span class="sxs-lookup"><span data-stu-id="5c816-103">visualInfo resource type</span></span>

<span data-ttu-id="5c816-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c816-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c816-105">Um tipo complexo para representar a propriedade **visualElements** no objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="5c816-105">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="5c816-106">Cada atividade do usuário será mostrada na linha do tempo como um cartão adaptável.</span><span class="sxs-lookup"><span data-stu-id="5c816-106">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="5c816-107">Os desenvolvedores de aplicativos são incentivados a fornecer um cartão personalizado que captura a essência da atividade que ocorreu no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c816-107">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="5c816-108">Isso é possível ao fornecer um cartão JSON personalizado na propriedade Content.</span><span class="sxs-lookup"><span data-stu-id="5c816-108">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="5c816-109">Além dos metadados visuais com um cartão adaptável, o aplicativo pode especificar metadados de conteúdo – dados que são usados para criar inferências sobre a atividade do usuário para oferecer novas atividades para o reenvolvimento futuro.</span><span class="sxs-lookup"><span data-stu-id="5c816-109">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="5c816-110">Isso é possível usando a propriedade contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades do schema.org para descrever o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5c816-110">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="5c816-111">Se um cartão personalizado não for fornecido, um cartão simples será gerado usando as propriedades displayText e Description.</span><span class="sxs-lookup"><span data-stu-id="5c816-111">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="5c816-112">Os cartões personalizados são recomendados para exibir o melhor conteúdo de dentro de seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5c816-112">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="5c816-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c816-113">Properties</span></span>

|<span data-ttu-id="5c816-114">Nome</span><span class="sxs-lookup"><span data-stu-id="5c816-114">Name</span></span> | <span data-ttu-id="5c816-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c816-115">Type</span></span> | <span data-ttu-id="5c816-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c816-116">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="5c816-117">displayText</span><span class="sxs-lookup"><span data-stu-id="5c816-117">displayText</span></span> | <span data-ttu-id="5c816-118">String</span><span class="sxs-lookup"><span data-stu-id="5c816-118">String</span></span> | <span data-ttu-id="5c816-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c816-119">Required.</span></span> <span data-ttu-id="5c816-120">Descrição de texto curto da atividade exclusiva do usuário (por exemplo, nome do documento em casos em que uma atividade refere-se à criação de documentos)</span><span class="sxs-lookup"><span data-stu-id="5c816-120">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="5c816-121">description</span><span class="sxs-lookup"><span data-stu-id="5c816-121">description</span></span> | <span data-ttu-id="5c816-122">String</span><span class="sxs-lookup"><span data-stu-id="5c816-122">String</span></span> | <span data-ttu-id="5c816-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c816-123">Optional.</span></span> <span data-ttu-id="5c816-124">Descrição de texto mais longa da atividade exclusiva do usuário (exemplo: nome do documento, primeira frase e/ou metadados)</span><span class="sxs-lookup"><span data-stu-id="5c816-124">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="5c816-125">CorDoFundo</span><span class="sxs-lookup"><span data-stu-id="5c816-125">backgroundColor</span></span> | <span data-ttu-id="5c816-126">String</span><span class="sxs-lookup"><span data-stu-id="5c816-126">String</span></span> | <span data-ttu-id="5c816-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c816-127">Optional.</span></span> <span data-ttu-id="5c816-128">Cor de plano de fundo usada para renderizar a atividade na cor da marca de interface do usuário da origem do aplicativo da atividade.</span><span class="sxs-lookup"><span data-stu-id="5c816-128">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="5c816-129">Deve ser uma cor hexadecimal válida</span><span class="sxs-lookup"><span data-stu-id="5c816-129">Must be a valid hex color</span></span>|
|<span data-ttu-id="5c816-130">conteúdo</span><span class="sxs-lookup"><span data-stu-id="5c816-130">content</span></span> | <span data-ttu-id="5c816-131">Objeto JSON não digitado</span><span class="sxs-lookup"><span data-stu-id="5c816-131">Untyped JSON object</span></span> | <span data-ttu-id="5c816-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c816-132">Optional.</span></span> <span data-ttu-id="5c816-133">Parte personalizada de dados-objeto JSON usado para fornecer conteúdo personalizado para renderizar a atividade na interface do usuário do shell do Windows</span><span class="sxs-lookup"><span data-stu-id="5c816-133">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="5c816-134">attribution</span><span class="sxs-lookup"><span data-stu-id="5c816-134">attribution</span></span> | [<span data-ttu-id="5c816-135">imageInfo</span><span class="sxs-lookup"><span data-stu-id="5c816-135">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="5c816-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5c816-136">Optional.</span></span> <span data-ttu-id="5c816-137">Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="5c816-137">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c816-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c816-138">JSON Representation</span></span>

<span data-ttu-id="5c816-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c816-139">The following is a JSON representation of the resource.</span></span>

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
