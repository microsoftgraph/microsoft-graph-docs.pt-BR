---
title: tipo de recurso addwatermarkaction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ba3bd679d01d31aec779071a766ab804761e614
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939163"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="41eaa-103">tipo de recurso addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="41eaa-103">addWatermarkAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41eaa-104">Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="41eaa-104">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="41eaa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41eaa-105">Properties</span></span>

| <span data-ttu-id="41eaa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41eaa-106">Property</span></span>      | <span data-ttu-id="41eaa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="41eaa-107">Type</span></span>   | <span data-ttu-id="41eaa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="41eaa-108">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="41eaa-109">fontColor</span><span class="sxs-lookup"><span data-stu-id="41eaa-109">fontColor</span></span>     | <span data-ttu-id="41eaa-110">String</span><span class="sxs-lookup"><span data-stu-id="41eaa-110">String</span></span> | <span data-ttu-id="41eaa-111">Cor da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="41eaa-111">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="41eaa-112">fontName</span><span class="sxs-lookup"><span data-stu-id="41eaa-112">fontName</span></span>      | <span data-ttu-id="41eaa-113">String</span><span class="sxs-lookup"><span data-stu-id="41eaa-113">String</span></span> | <span data-ttu-id="41eaa-114">Nome da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="41eaa-114">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="41eaa-115">fontSize</span><span class="sxs-lookup"><span data-stu-id="41eaa-115">fontSize</span></span>      | <span data-ttu-id="41eaa-116">Int32</span><span class="sxs-lookup"><span data-stu-id="41eaa-116">Int32</span></span>  | <span data-ttu-id="41eaa-117">Tamanho da fonte a ser usado para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="41eaa-117">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="41eaa-118">teclado</span><span class="sxs-lookup"><span data-stu-id="41eaa-118">layout</span></span>        | <span data-ttu-id="41eaa-119">String</span><span class="sxs-lookup"><span data-stu-id="41eaa-119">String</span></span> | <span data-ttu-id="41eaa-120">Os valores possíveis são: `horizontal` e `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="41eaa-120">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="41eaa-121">texto</span><span class="sxs-lookup"><span data-stu-id="41eaa-121">text</span></span>          | <span data-ttu-id="41eaa-122">String</span><span class="sxs-lookup"><span data-stu-id="41eaa-122">String</span></span> | <span data-ttu-id="41eaa-123">O conteúdo da própria marca d' água.</span><span class="sxs-lookup"><span data-stu-id="41eaa-123">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="41eaa-124">uiElementname</span><span class="sxs-lookup"><span data-stu-id="41eaa-124">uiElementName</span></span> | <span data-ttu-id="41eaa-125">String</span><span class="sxs-lookup"><span data-stu-id="41eaa-125">String</span></span> | <span data-ttu-id="41eaa-126">O nome do elemento de interface do usuário onde a marca d' água deve ser colocada.</span><span class="sxs-lookup"><span data-stu-id="41eaa-126">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41eaa-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41eaa-127">JSON representation</span></span>

<span data-ttu-id="41eaa-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41eaa-128">The following is a JSON representation of the resource.</span></span>

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