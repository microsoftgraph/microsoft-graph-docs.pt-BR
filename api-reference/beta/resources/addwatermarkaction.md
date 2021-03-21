---
title: Tipo de recurso addWatermarkAction
description: Representa uma ação que especifica os detalhes sobre a marca d'água do conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962123"
---
# <a name="addwatermarkaction-resource-type"></a><span data-ttu-id="b2f93-103">Tipo de recurso addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="b2f93-103">addWatermarkAction resource type</span></span>

<span data-ttu-id="b2f93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2f93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2f93-105">Representa uma ação que especifica os detalhes sobre a marca d'água do conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="b2f93-105">Represents an action that specifies the details on the content watermark to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="b2f93-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2f93-106">Properties</span></span>

| <span data-ttu-id="b2f93-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2f93-107">Property</span></span>      | <span data-ttu-id="b2f93-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2f93-108">Type</span></span>   | <span data-ttu-id="b2f93-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2f93-109">Description</span></span>                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| <span data-ttu-id="b2f93-110">fontColor</span><span class="sxs-lookup"><span data-stu-id="b2f93-110">fontColor</span></span>     | <span data-ttu-id="b2f93-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f93-111">String</span></span> | <span data-ttu-id="b2f93-112">Cor da fonte a ser usada para a marca d'água.</span><span class="sxs-lookup"><span data-stu-id="b2f93-112">Color of the font to use for the watermark.</span></span>                      |
| <span data-ttu-id="b2f93-113">fontName</span><span class="sxs-lookup"><span data-stu-id="b2f93-113">fontName</span></span>      | <span data-ttu-id="b2f93-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f93-114">String</span></span> | <span data-ttu-id="b2f93-115">Nome da fonte a ser usada para a marca d'água.</span><span class="sxs-lookup"><span data-stu-id="b2f93-115">Name of the font to use for the watermark.</span></span>                       |
| <span data-ttu-id="b2f93-116">fontSize</span><span class="sxs-lookup"><span data-stu-id="b2f93-116">fontSize</span></span>      | <span data-ttu-id="b2f93-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b2f93-117">Int32</span></span>  | <span data-ttu-id="b2f93-118">Tamanho da fonte a ser usado para a marca d'água.</span><span class="sxs-lookup"><span data-stu-id="b2f93-118">Font size to use for the watermark.</span></span>                              |
| <span data-ttu-id="b2f93-119">layout</span><span class="sxs-lookup"><span data-stu-id="b2f93-119">layout</span></span>        | <span data-ttu-id="b2f93-120">String</span><span class="sxs-lookup"><span data-stu-id="b2f93-120">String</span></span> | <span data-ttu-id="b2f93-121">Os valores possíveis são: `horizontal` e `diagonal`.</span><span class="sxs-lookup"><span data-stu-id="b2f93-121">Possible values are: `horizontal`, `diagonal`.</span></span>                   |
| <span data-ttu-id="b2f93-122">texto</span><span class="sxs-lookup"><span data-stu-id="b2f93-122">text</span></span>          | <span data-ttu-id="b2f93-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f93-123">String</span></span> | <span data-ttu-id="b2f93-124">O conteúdo da marca d'água em si.</span><span class="sxs-lookup"><span data-stu-id="b2f93-124">The contents of the watermark itself.</span></span>                            |
| <span data-ttu-id="b2f93-125">uiElementName</span><span class="sxs-lookup"><span data-stu-id="b2f93-125">uiElementName</span></span> | <span data-ttu-id="b2f93-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2f93-126">String</span></span> | <span data-ttu-id="b2f93-127">O nome do elemento da interface do usuário onde a marca d'água deve ser colocada.</span><span class="sxs-lookup"><span data-stu-id="b2f93-127">The name of the UI element where the watermark should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2f93-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2f93-128">JSON representation</span></span>

<span data-ttu-id="b2f93-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2f93-129">The following is a JSON representation of the resource.</span></span>

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

