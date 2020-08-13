---
title: tipo de recurso addwatermarkaction
description: Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a94f517fe9f5da207febf9e776643a7c17c18d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508398"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="280e8-103">tipo de recurso addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="280e8-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="280e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="280e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="280e8-105">Representa uma ação que especifica os detalhes sobre a marca d' água de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="280e8-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="280e8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="280e8-106">Properties</span></span>

| <span data-ttu-id="280e8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="280e8-107">Property</span></span>      | <span data-ttu-id="280e8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="280e8-108">Type</span></span>   | <span data-ttu-id="280e8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="280e8-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="280e8-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="280e8-110">fontColor</span></span>     | <span data-ttu-id="280e8-111">String</span><span class="sxs-lookup"><span data-stu-id="280e8-111">String</span></span> | <span data-ttu-id="280e8-112">Cor da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="280e8-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="280e8-113">fontName</span><span class="sxs-lookup"><span data-stu-id="280e8-113">fontName</span></span>      | <span data-ttu-id="280e8-114">String</span><span class="sxs-lookup"><span data-stu-id="280e8-114">String</span></span> | <span data-ttu-id="280e8-115">Nome da fonte a ser usada para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="280e8-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="280e8-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="280e8-116">fontSize</span></span>      | <span data-ttu-id="280e8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="280e8-117">Int32</span></span>  | <span data-ttu-id="280e8-118">Tamanho da fonte a ser usado para a marca d' água.</span><span class="sxs-lookup"><span data-stu-id="280e8-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="280e8-119">teclado</span><span class="sxs-lookup"><span data-stu-id="280e8-119">layout</span></span>        | <span data-ttu-id="280e8-120">String</span><span class="sxs-lookup"><span data-stu-id="280e8-120">String</span></span> | <span data-ttu-id="280e8-121">Os valores possíveis são: `horizontal` e `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="280e8-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="280e8-122">texto</span><span class="sxs-lookup"><span data-stu-id="280e8-122">text</span></span>          | <span data-ttu-id="280e8-123">String</span><span class="sxs-lookup"><span data-stu-id="280e8-123">String</span></span> | <span data-ttu-id="280e8-124">O conteúdo da própria marca d' água.</span><span class="sxs-lookup"><span data-stu-id="280e8-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="280e8-125">uiElementname</span><span class="sxs-lookup"><span data-stu-id="280e8-125">uiElementName</span></span> | <span data-ttu-id="280e8-126">String</span><span class="sxs-lookup"><span data-stu-id="280e8-126">String</span></span> | <span data-ttu-id="280e8-127">O nome do elemento de interface do usuário onde a marca d' água deve ser colocada.</span><span class="sxs-lookup"><span data-stu-id="280e8-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="280e8-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="280e8-128">JSON representation</span></span>

<span data-ttu-id="280e8-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="280e8-129">The following is a JSON representation of the resource.</span></span>

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