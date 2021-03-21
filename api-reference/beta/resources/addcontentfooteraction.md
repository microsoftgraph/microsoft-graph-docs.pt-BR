---
title: Tipo de recurso addContentFooterAction
description: Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem adicionados às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 20debce7dc408bd10d4f62b905efa55156d4d4ca
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962131"
---
# <a name="addcontentfooteraction-resource-type"></a><span data-ttu-id="5a6ab-103">Tipo de recurso addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="5a6ab-103">addContentFooterAction resource type</span></span>

<span data-ttu-id="5a6ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a6ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a6ab-105">Representa uma ação que especifica os detalhes no rodapé de conteúdo a serem adicionados às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-105">Represents an action that specifies the details on the content footer to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="5a6ab-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a6ab-106">Properties</span></span>

| <span data-ttu-id="5a6ab-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a6ab-107">Property</span></span>      | <span data-ttu-id="5a6ab-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a6ab-108">Type</span></span>   | <span data-ttu-id="5a6ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a6ab-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="5a6ab-110">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="5a6ab-110">alignment</span></span>     | <span data-ttu-id="5a6ab-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a6ab-111">String</span></span> | <span data-ttu-id="5a6ab-112">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="5a6ab-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="5a6ab-113">fontColor</span></span>     | <span data-ttu-id="5a6ab-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a6ab-114">String</span></span> | <span data-ttu-id="5a6ab-115">Cor da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-115">Color of the font to use for the footer.</span></span>                      |
| <span data-ttu-id="5a6ab-116">fontName</span><span class="sxs-lookup"><span data-stu-id="5a6ab-116">fontName</span></span>      | <span data-ttu-id="5a6ab-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a6ab-117">String</span></span> | <span data-ttu-id="5a6ab-118">Nome da fonte a ser usada para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-118">Name of the font to use for the footer.</span></span>                       |
| <span data-ttu-id="5a6ab-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="5a6ab-119">fontSize</span></span>      | <span data-ttu-id="5a6ab-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5a6ab-120">Int32</span></span>  | <span data-ttu-id="5a6ab-121">Tamanho da fonte a ser usado para o rodapé.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-121">Font size to use for the footer.</span></span>                              |
| <span data-ttu-id="5a6ab-122">margin</span><span class="sxs-lookup"><span data-stu-id="5a6ab-122">margin</span></span>        | <span data-ttu-id="5a6ab-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5a6ab-123">Int32</span></span>  | <span data-ttu-id="5a6ab-124">A margem do header na parte inferior do documento.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-124">The margin of the header from the bottom of the document.</span></span>     |
| <span data-ttu-id="5a6ab-125">texto</span><span class="sxs-lookup"><span data-stu-id="5a6ab-125">text</span></span>          | <span data-ttu-id="5a6ab-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a6ab-126">String</span></span> | <span data-ttu-id="5a6ab-127">O conteúdo do rodapé em si.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-127">The contents of the footer itself.</span></span>                            |
| <span data-ttu-id="5a6ab-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="5a6ab-128">uiElementName</span></span> | <span data-ttu-id="5a6ab-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a6ab-129">String</span></span> | <span data-ttu-id="5a6ab-130">O nome do elemento da interface do usuário onde o rodapé deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-130">The name of the UI element where the footer should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a6ab-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a6ab-131">JSON representation</span></span>

<span data-ttu-id="5a6ab-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a6ab-132">The following is a JSON representation of the resource.</span></span>

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

