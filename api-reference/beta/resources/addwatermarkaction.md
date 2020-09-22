---
title: tipo de recurso addwatermarkaction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 884553ce1181fd3d79fe0e953fe7703b386698b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024427"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="d34b5-103">tipo de recurso addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="d34b5-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="d34b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d34b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d34b5-105">Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="d34b5-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="d34b5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d34b5-106">Properties</span></span>

| <span data-ttu-id="d34b5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d34b5-107">Property</span></span>      | <span data-ttu-id="d34b5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d34b5-108">Type</span></span>   | <span data-ttu-id="d34b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d34b5-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="d34b5-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="d34b5-110">fontColor</span></span>     | <span data-ttu-id="d34b5-111">String</span><span class="sxs-lookup"><span data-stu-id="d34b5-111">String</span></span> | <span data-ttu-id="d34b5-112">Cor da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="d34b5-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="d34b5-113">fontName</span><span class="sxs-lookup"><span data-stu-id="d34b5-113">fontName</span></span>      | <span data-ttu-id="d34b5-114">String</span><span class="sxs-lookup"><span data-stu-id="d34b5-114">String</span></span> | <span data-ttu-id="d34b5-115">Nome da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="d34b5-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="d34b5-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="d34b5-116">fontSize</span></span>      | <span data-ttu-id="d34b5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d34b5-117">Int32</span></span>  | <span data-ttu-id="d34b5-118">Tamanho da fonte a ser usado para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="d34b5-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="d34b5-119">teclado</span><span class="sxs-lookup"><span data-stu-id="d34b5-119">layout</span></span>        | <span data-ttu-id="d34b5-120">String</span><span class="sxs-lookup"><span data-stu-id="d34b5-120">String</span></span> | <span data-ttu-id="d34b5-121">Os valores possíveis são: `horizontal` e `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="d34b5-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="d34b5-122">texto</span><span class="sxs-lookup"><span data-stu-id="d34b5-122">text</span></span>          | <span data-ttu-id="d34b5-123">String</span><span class="sxs-lookup"><span data-stu-id="d34b5-123">String</span></span> | <span data-ttu-id="d34b5-124">O conteúdo da própria marca d' água.</span><span class="sxs-lookup"><span data-stu-id="d34b5-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="d34b5-125">uiElementname</span><span class="sxs-lookup"><span data-stu-id="d34b5-125">uiElementName</span></span> | <span data-ttu-id="d34b5-126">String</span><span class="sxs-lookup"><span data-stu-id="d34b5-126">String</span></span> | <span data-ttu-id="d34b5-127">O nome do elemento de interface do usuário onde a marca d' água deve ser colocada.</span><span class="sxs-lookup"><span data-stu-id="d34b5-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d34b5-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d34b5-128">JSON representation</span></span>

<span data-ttu-id="d34b5-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d34b5-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

