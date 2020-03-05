---
title: tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05bbd7ee4b2d4b2b9c4e772b19bd26c86d91cc69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508419"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="e881a-103">tipo de recurso addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="e881a-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="e881a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e881a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e881a-105">Representa uma ação que especifica os detalhes no rodapé de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="e881a-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="e881a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e881a-106">Properties</span></span>

| <span data-ttu-id="e881a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e881a-107">Property</span></span>      | <span data-ttu-id="e881a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e881a-108">Type</span></span>   | <span data-ttu-id="e881a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e881a-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="e881a-110">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="e881a-110">alignment</span></span>     | <span data-ttu-id="e881a-111">String</span><span class="sxs-lookup"><span data-stu-id="e881a-111">String</span></span> | <span data-ttu-id="e881a-112">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="e881a-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="e881a-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="e881a-113">fontColor</span></span>     | <span data-ttu-id="e881a-114">String</span><span class="sxs-lookup"><span data-stu-id="e881a-114">String</span></span> | <span data-ttu-id="e881a-115">Cor da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="e881a-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="e881a-116">fontName</span><span class="sxs-lookup"><span data-stu-id="e881a-116">fontName</span></span>      | <span data-ttu-id="e881a-117">String</span><span class="sxs-lookup"><span data-stu-id="e881a-117">String</span></span> | <span data-ttu-id="e881a-118">Nome da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="e881a-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="e881a-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="e881a-119">fontSize</span></span>      | <span data-ttu-id="e881a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e881a-120">Int32</span></span>  | <span data-ttu-id="e881a-121">Tamanho da fonte a ser usado para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="e881a-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="e881a-122">Margin</span><span class="sxs-lookup"><span data-stu-id="e881a-122">margin</span></span>        | <span data-ttu-id="e881a-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e881a-123">Int32</span></span>  | <span data-ttu-id="e881a-124">A margem do cabeçalho na parte inferior do documento.</span><span class="sxs-lookup"><span data-stu-id="e881a-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="e881a-125">texto</span><span class="sxs-lookup"><span data-stu-id="e881a-125">text</span></span>          | <span data-ttu-id="e881a-126">String</span><span class="sxs-lookup"><span data-stu-id="e881a-126">String</span></span> | <span data-ttu-id="e881a-127">O conteúdo do rodapé propriamente dito.</span><span class="sxs-lookup"><span data-stu-id="e881a-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="e881a-128">uiElementname</span><span class="sxs-lookup"><span data-stu-id="e881a-128">uiElementName</span></span> | <span data-ttu-id="e881a-129">String</span><span class="sxs-lookup"><span data-stu-id="e881a-129">String</span></span> | <span data-ttu-id="e881a-130">O nome do elemento de interface do usuário onde o rodapé deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="e881a-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e881a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e881a-131">JSON representation</span></span>

<span data-ttu-id="e881a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e881a-132">The following is a JSON representation of the resource.</span></span>

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