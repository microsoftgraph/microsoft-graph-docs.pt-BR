---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: d4ed317b987d461c9ef6816e9d05aae0de358ec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037196"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="b9bd3-103">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="b9bd3-103">imageInfo resource type</span></span>

<span data-ttu-id="b9bd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9bd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9bd3-105">Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="b9bd3-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="b9bd3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9bd3-106">Properties</span></span>

|<span data-ttu-id="b9bd3-107">Nome</span><span class="sxs-lookup"><span data-stu-id="b9bd3-107">Name</span></span> | <span data-ttu-id="b9bd3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9bd3-108">Type</span></span> | <span data-ttu-id="b9bd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9bd3-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b9bd3-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="b9bd3-110">iconUrl</span></span> | <span data-ttu-id="b9bd3-111">String</span><span class="sxs-lookup"><span data-stu-id="b9bd3-111">String</span></span> | <span data-ttu-id="b9bd3-112">Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="b9bd3-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="b9bd3-113">alternateText</span><span class="sxs-lookup"><span data-stu-id="b9bd3-113">alternateText</span></span> | <span data-ttu-id="b9bd3-114">String</span><span class="sxs-lookup"><span data-stu-id="b9bd3-114">String</span></span> | <span data-ttu-id="b9bd3-115">Opcion Alt-conteúdo de texto acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="b9bd3-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="b9bd3-116">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="b9bd3-116">addImageQuery</span></span> | <span data-ttu-id="b9bd3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9bd3-117">Boolean</span></span> | <span data-ttu-id="b9bd3-118">Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="b9bd3-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="b9bd3-119">Por exemplo, uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="b9bd3-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9bd3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9bd3-120">JSON Representation</span></span>

<span data-ttu-id="b9bd3-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b9bd3-121">Here is a JSON representation of the resource</span></span>

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

