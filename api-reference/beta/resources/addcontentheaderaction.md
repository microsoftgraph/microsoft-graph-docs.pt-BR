---
title: tipo de recurso addContentHeaderAction
description: Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 341af43f03d8a319c7aaec535681f21db0a7f7f4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939099"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="4fbe2-103">tipo de recurso addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="4fbe2-103">addContentHeaderAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fbe2-104">Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-104">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="4fbe2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fbe2-105">Properties</span></span>

| <span data-ttu-id="4fbe2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fbe2-106">Property</span></span>      | <span data-ttu-id="4fbe2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fbe2-107">Type</span></span>   | <span data-ttu-id="4fbe2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbe2-108">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="4fbe2-109">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="4fbe2-109">alignment</span></span>     | <span data-ttu-id="4fbe2-110">String</span><span class="sxs-lookup"><span data-stu-id="4fbe2-110">String</span></span> | <span data-ttu-id="4fbe2-111">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-111">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="4fbe2-112">fontColor</span><span class="sxs-lookup"><span data-stu-id="4fbe2-112">fontColor</span></span>     | <span data-ttu-id="4fbe2-113">String</span><span class="sxs-lookup"><span data-stu-id="4fbe2-113">String</span></span> | <span data-ttu-id="4fbe2-114">Cor da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-114">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="4fbe2-115">fontName</span><span class="sxs-lookup"><span data-stu-id="4fbe2-115">fontName</span></span>      | <span data-ttu-id="4fbe2-116">String</span><span class="sxs-lookup"><span data-stu-id="4fbe2-116">String</span></span> | <span data-ttu-id="4fbe2-117">Nome da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-117">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="4fbe2-118">fontSize</span><span class="sxs-lookup"><span data-stu-id="4fbe2-118">fontSize</span></span>      | <span data-ttu-id="4fbe2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="4fbe2-119">Int32</span></span>  | <span data-ttu-id="4fbe2-120">Tamanho da fonte a ser usado para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-120">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="4fbe2-121">Margin</span><span class="sxs-lookup"><span data-stu-id="4fbe2-121">margin</span></span>        | <span data-ttu-id="4fbe2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4fbe2-122">Int32</span></span>  | <span data-ttu-id="4fbe2-123">A margem do cabeçalho na parte superior do documento.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-123">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="4fbe2-124">texto</span><span class="sxs-lookup"><span data-stu-id="4fbe2-124">text</span></span>          | <span data-ttu-id="4fbe2-125">String</span><span class="sxs-lookup"><span data-stu-id="4fbe2-125">String</span></span> | <span data-ttu-id="4fbe2-126">O conteúdo do próprio cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-126">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="4fbe2-127">uiElementname</span><span class="sxs-lookup"><span data-stu-id="4fbe2-127">uiElementName</span></span> | <span data-ttu-id="4fbe2-128">String</span><span class="sxs-lookup"><span data-stu-id="4fbe2-128">String</span></span> | <span data-ttu-id="4fbe2-129">O nome do elemento de interface do usuário onde o cabeçalho deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-129">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4fbe2-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fbe2-130">JSON representation</span></span>

<span data-ttu-id="4fbe2-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4fbe2-131">The following is a JSON representation of the resource.</span></span>

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