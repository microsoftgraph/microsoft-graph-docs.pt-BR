---
title: Tipo de recurso addContentHeaderAction
description: Representa uma ação que especifica os detalhes do header de conteúdo a serem adicionados às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 65754bffc034611fd319403cd81d931addfea9f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962130"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="ef3cf-103">Tipo de recurso addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="ef3cf-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="ef3cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef3cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef3cf-105">Representa uma ação que especifica os detalhes do header de conteúdo a serem adicionados às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="ef3cf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef3cf-106">Properties</span></span>

| <span data-ttu-id="ef3cf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef3cf-107">Property</span></span>      | <span data-ttu-id="ef3cf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef3cf-108">Type</span></span>   | <span data-ttu-id="ef3cf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef3cf-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="ef3cf-110">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="ef3cf-110">alignment</span></span>     | <span data-ttu-id="ef3cf-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef3cf-111">String</span></span> | <span data-ttu-id="ef3cf-112">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="ef3cf-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="ef3cf-113">fontColor</span></span>     | <span data-ttu-id="ef3cf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef3cf-114">String</span></span> | <span data-ttu-id="ef3cf-115">Cor da fonte a ser usada para o header.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="ef3cf-116">fontName</span><span class="sxs-lookup"><span data-stu-id="ef3cf-116">fontName</span></span>      | <span data-ttu-id="ef3cf-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef3cf-117">String</span></span> | <span data-ttu-id="ef3cf-118">Nome da fonte a ser usada para o header.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="ef3cf-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="ef3cf-119">fontSize</span></span>      | <span data-ttu-id="ef3cf-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ef3cf-120">Int32</span></span>  | <span data-ttu-id="ef3cf-121">Tamanho da fonte a ser usado para o header.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="ef3cf-122">margin</span><span class="sxs-lookup"><span data-stu-id="ef3cf-122">margin</span></span>        | <span data-ttu-id="ef3cf-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ef3cf-123">Int32</span></span>  | <span data-ttu-id="ef3cf-124">A margem do header na parte superior do documento.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="ef3cf-125">texto</span><span class="sxs-lookup"><span data-stu-id="ef3cf-125">text</span></span>          | <span data-ttu-id="ef3cf-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef3cf-126">String</span></span> | <span data-ttu-id="ef3cf-127">O conteúdo do próprio header.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="ef3cf-128">uiElementName</span><span class="sxs-lookup"><span data-stu-id="ef3cf-128">uiElementName</span></span> | <span data-ttu-id="ef3cf-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef3cf-129">String</span></span> | <span data-ttu-id="ef3cf-130">O nome do elemento da interface do usuário onde o header deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef3cf-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef3cf-131">JSON representation</span></span>

<span data-ttu-id="ef3cf-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef3cf-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
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
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

