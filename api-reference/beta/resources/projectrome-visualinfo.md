---
title: tipo de recurso de visualInfo
description: Um tipo complexo para representar a propriedade **visualElements** no objeto de atividade.
localization_priority: Normal
ms.openlocfilehash: 3e1dd3d7e4ecfaf5053f839f0ac0d0039692b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855311"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="5cf8f-103">tipo de recurso de visualInfo</span><span class="sxs-lookup"><span data-stu-id="5cf8f-103">visualInfo resource type</span></span>

> <span data-ttu-id="5cf8f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cf8f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cf8f-106">Um tipo complexo para representar a propriedade **visualElements** no objeto de [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="5cf8f-106">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="5cf8f-107">Cada atividade do usuário será exibida na linha do tempo como um cartão adaptável.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-107">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="5cf8f-108">Desenvolvedores de aplicativos são incentivados a fornecer um cartão personalizado que captura a essência da atividade que foi realizada no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-108">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="5cf8f-109">Isso é possível, fornecendo um cartão JSON personalizado na propriedade conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-109">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="5cf8f-110">Além dos metadados visual com uma placa adaptável, app pode especificar metadados do conteúdo – dados a ser usado para construir Inferências sobre a atividade do usuário a fim de oferecer novas atividades para o compromisso re futura.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-110">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="5cf8f-111">Isso é possível usando a propriedade de contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades de schema.org para descrever o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-111">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="5cf8f-112">Se não for fornecido um cartão personalizado, será gerado um cartão simple usando propriedades displayText e descrição.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-112">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="5cf8f-113">Cartões personalizados são recomendados para demonstrar o melhor conteúdo de dentro de seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-113">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="5cf8f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cf8f-114">Properties</span></span>

|<span data-ttu-id="5cf8f-115">Nome</span><span class="sxs-lookup"><span data-stu-id="5cf8f-115">Name</span></span> | <span data-ttu-id="5cf8f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cf8f-116">Type</span></span> | <span data-ttu-id="5cf8f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf8f-117">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="5cf8f-118">displayText</span><span class="sxs-lookup"><span data-stu-id="5cf8f-118">displayText</span></span> | <span data-ttu-id="5cf8f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf8f-119">String</span></span> | <span data-ttu-id="5cf8f-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-120">Required.</span></span> <span data-ttu-id="5cf8f-121">Uma breve descrição de texto de atividade de exclusivo do usuário (por exemplo, nome do documento em casos onde uma atividade refere-se a criação de documentos)</span><span class="sxs-lookup"><span data-stu-id="5cf8f-121">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="5cf8f-122">description</span><span class="sxs-lookup"><span data-stu-id="5cf8f-122">description</span></span> | <span data-ttu-id="5cf8f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf8f-123">String</span></span> | <span data-ttu-id="5cf8f-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-124">Optional.</span></span> <span data-ttu-id="5cf8f-125">Descrição de texto mais longa da atividade exclusivo do usuário (exemplo: nome, primeira frase e/ou metadados de documentos)</span><span class="sxs-lookup"><span data-stu-id="5cf8f-125">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="5cf8f-126">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="5cf8f-126">backgroundColor</span></span> | <span data-ttu-id="5cf8f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5cf8f-127">String</span></span> | <span data-ttu-id="5cf8f-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-128">Optional.</span></span> <span data-ttu-id="5cf8f-129">Cor de plano de fundo usada para processar a atividade na interface do usuário - cor de marca para a fonte da atividade do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-129">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="5cf8f-130">Deve ser uma cor hexadecimal válida</span><span class="sxs-lookup"><span data-stu-id="5cf8f-130">Must be a valid hex color</span></span>|
|<span data-ttu-id="5cf8f-131">content</span><span class="sxs-lookup"><span data-stu-id="5cf8f-131">content</span></span> | <span data-ttu-id="5cf8f-132">Objeto sem JSON</span><span class="sxs-lookup"><span data-stu-id="5cf8f-132">Untyped JSON object</span></span> | <span data-ttu-id="5cf8f-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-133">Optional.</span></span> <span data-ttu-id="5cf8f-134">Parte personalizada de dados - objeto JSON usados para fornecer conteúdo personalizado para renderizar a atividade no UI do Shell do Windows</span><span class="sxs-lookup"><span data-stu-id="5cf8f-134">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="5cf8f-135">attribution</span><span class="sxs-lookup"><span data-stu-id="5cf8f-135">attribution</span></span> | [<span data-ttu-id="5cf8f-136">imageInfo</span><span class="sxs-lookup"><span data-stu-id="5cf8f-136">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="5cf8f-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-137">Optional.</span></span> <span data-ttu-id="5cf8f-138">Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="5cf8f-138">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cf8f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cf8f-139">JSON Representation</span></span>

<span data-ttu-id="5cf8f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cf8f-140">The following is a JSON representation of the resource.</span></span>

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
    "@data.type": "microsoft.graph.visualInfo",
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
        "@data.type": "microsoft.graph.Json"
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
