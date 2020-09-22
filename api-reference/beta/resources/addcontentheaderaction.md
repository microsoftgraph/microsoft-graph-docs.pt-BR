---
title: tipo de recurso addContentHeaderAction
description: Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e7a5675cdf150f03b283f664e248319d49c820d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024512"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="e2cb9-103">tipo de recurso addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="e2cb9-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="e2cb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2cb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2cb9-105">Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="e2cb9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2cb9-106">Properties</span></span>

| <span data-ttu-id="e2cb9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2cb9-107">Property</span></span>      | <span data-ttu-id="e2cb9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2cb9-108">Type</span></span>   | <span data-ttu-id="e2cb9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2cb9-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="e2cb9-110">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="e2cb9-110">alignment</span></span>     | <span data-ttu-id="e2cb9-111">String</span><span class="sxs-lookup"><span data-stu-id="e2cb9-111">String</span></span> | <span data-ttu-id="e2cb9-112">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="e2cb9-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="e2cb9-113">fontColor</span></span>     | <span data-ttu-id="e2cb9-114">String</span><span class="sxs-lookup"><span data-stu-id="e2cb9-114">String</span></span> | <span data-ttu-id="e2cb9-115">Cor da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="e2cb9-116">fontName</span><span class="sxs-lookup"><span data-stu-id="e2cb9-116">fontName</span></span>      | <span data-ttu-id="e2cb9-117">String</span><span class="sxs-lookup"><span data-stu-id="e2cb9-117">String</span></span> | <span data-ttu-id="e2cb9-118">Nome da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="e2cb9-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="e2cb9-119">fontSize</span></span>      | <span data-ttu-id="e2cb9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cb9-120">Int32</span></span>  | <span data-ttu-id="e2cb9-121">Tamanho da fonte a ser usado para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="e2cb9-122">margin</span><span class="sxs-lookup"><span data-stu-id="e2cb9-122">margin</span></span>        | <span data-ttu-id="e2cb9-123">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cb9-123">Int32</span></span>  | <span data-ttu-id="e2cb9-124">A margem do cabeçalho na parte superior do documento.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="e2cb9-125">texto</span><span class="sxs-lookup"><span data-stu-id="e2cb9-125">text</span></span>          | <span data-ttu-id="e2cb9-126">String</span><span class="sxs-lookup"><span data-stu-id="e2cb9-126">String</span></span> | <span data-ttu-id="e2cb9-127">O conteúdo do próprio cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="e2cb9-128">uiElementname</span><span class="sxs-lookup"><span data-stu-id="e2cb9-128">uiElementName</span></span> | <span data-ttu-id="e2cb9-129">String</span><span class="sxs-lookup"><span data-stu-id="e2cb9-129">String</span></span> | <span data-ttu-id="e2cb9-130">O nome do elemento de interface do usuário onde o cabeçalho deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2cb9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2cb9-131">JSON representation</span></span>

<span data-ttu-id="e2cb9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2cb9-132">The following is a JSON representation of the resource.</span></span>

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

