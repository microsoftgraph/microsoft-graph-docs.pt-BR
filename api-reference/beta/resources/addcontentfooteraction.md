---
title: tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b1a2cb0f3e2ffbfb5554c4ae0323cf4fd028e0c8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939100"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="b0dfd-103">tipo de recurso addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="b0dfd-103">addContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0dfd-104">Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-104">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="b0dfd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0dfd-105">Properties</span></span>

| <span data-ttu-id="b0dfd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0dfd-106">Property</span></span>      | <span data-ttu-id="b0dfd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0dfd-107">Type</span></span>   | <span data-ttu-id="b0dfd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0dfd-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="b0dfd-109">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="b0dfd-109">alignment</span></span>     | <span data-ttu-id="b0dfd-110">String</span><span class="sxs-lookup"><span data-stu-id="b0dfd-110">String</span></span> | <span data-ttu-id="b0dfd-111">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="b0dfd-112">fontColor</span><span class="sxs-lookup"><span data-stu-id="b0dfd-112">fontColor</span></span>     | <span data-ttu-id="b0dfd-113">String</span><span class="sxs-lookup"><span data-stu-id="b0dfd-113">String</span></span> | <span data-ttu-id="b0dfd-114">Cor da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-114">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="b0dfd-115">fontName</span><span class="sxs-lookup"><span data-stu-id="b0dfd-115">fontName</span></span>      | <span data-ttu-id="b0dfd-116">String</span><span class="sxs-lookup"><span data-stu-id="b0dfd-116">String</span></span> | <span data-ttu-id="b0dfd-117">Nome da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-117">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="b0dfd-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="b0dfd-118">fontSize</span></span>      | <span data-ttu-id="b0dfd-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b0dfd-119">Int32</span></span>  | <span data-ttu-id="b0dfd-120">Tamanho da fonte a ser usado para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-120">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="b0dfd-121">Margin</span><span class="sxs-lookup"><span data-stu-id="b0dfd-121">margin</span></span>        | <span data-ttu-id="b0dfd-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b0dfd-122">Int32</span></span>  | <span data-ttu-id="b0dfd-123">A margem do cabeçalho na parte inferior do documento.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-123">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="b0dfd-124">texto</span><span class="sxs-lookup"><span data-stu-id="b0dfd-124">text</span></span>          | <span data-ttu-id="b0dfd-125">String</span><span class="sxs-lookup"><span data-stu-id="b0dfd-125">String</span></span> | <span data-ttu-id="b0dfd-126">O conteúdo do rodapé propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-126">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="b0dfd-127">uiElementname</span><span class="sxs-lookup"><span data-stu-id="b0dfd-127">uiElementName</span></span> | <span data-ttu-id="b0dfd-128">String</span><span class="sxs-lookup"><span data-stu-id="b0dfd-128">String</span></span> | <span data-ttu-id="b0dfd-129">O nome do elemento de interface do usuário onde o rodapé deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-129">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0dfd-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0dfd-130">JSON representation</span></span>

<span data-ttu-id="b0dfd-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0dfd-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->