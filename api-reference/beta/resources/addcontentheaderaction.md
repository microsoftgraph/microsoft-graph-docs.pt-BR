---
title: tipo de recurso addContentHeaderAction
description: Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d426252b6ab83557c3d3085ac4ffa7a530aae271
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508405"
---
# <a name="addcontentheaderaction-resource-type"></a><span data-ttu-id="6e60e-103">tipo de recurso addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="6e60e-103">addContentHeaderAction resource type</span></span>

<span data-ttu-id="6e60e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e60e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e60e-105">Representa uma ação que especifica os detalhes sobre o cabeçalho de conteúdo a ser adicionado às informações, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="6e60e-105">Represents an action that specifies the details on the content header to be added to the information, if applicable.</span></span>

## <a name="properties"></a><span data-ttu-id="6e60e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e60e-106">Properties</span></span>

| <span data-ttu-id="6e60e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e60e-107">Property</span></span>      | <span data-ttu-id="6e60e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e60e-108">Type</span></span>   | <span data-ttu-id="6e60e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e60e-109">Description</span></span>                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| <span data-ttu-id="6e60e-110">Alinhamento</span><span class="sxs-lookup"><span data-stu-id="6e60e-110">alignment</span></span>     | <span data-ttu-id="6e60e-111">String</span><span class="sxs-lookup"><span data-stu-id="6e60e-111">String</span></span> | <span data-ttu-id="6e60e-112">Os valores possíveis são: `left`, `right`, `center`.</span><span class="sxs-lookup"><span data-stu-id="6e60e-112">Possible values are: `left`, `right`, `center`.</span></span>               |
| <span data-ttu-id="6e60e-113">fontColor</span><span class="sxs-lookup"><span data-stu-id="6e60e-113">fontColor</span></span>     | <span data-ttu-id="6e60e-114">String</span><span class="sxs-lookup"><span data-stu-id="6e60e-114">String</span></span> | <span data-ttu-id="6e60e-115">Cor da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6e60e-115">Color of the font to use for the header.</span></span>                      |
| <span data-ttu-id="6e60e-116">fontName</span><span class="sxs-lookup"><span data-stu-id="6e60e-116">fontName</span></span>      | <span data-ttu-id="6e60e-117">String</span><span class="sxs-lookup"><span data-stu-id="6e60e-117">String</span></span> | <span data-ttu-id="6e60e-118">Nome da fonte a ser usada para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6e60e-118">Name of the font to use for the header.</span></span>                       |
| <span data-ttu-id="6e60e-119">fontSize</span><span class="sxs-lookup"><span data-stu-id="6e60e-119">fontSize</span></span>      | <span data-ttu-id="6e60e-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6e60e-120">Int32</span></span>  | <span data-ttu-id="6e60e-121">Tamanho da fonte a ser usado para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6e60e-121">Font size to use for the header.</span></span>                              |
| <span data-ttu-id="6e60e-122">Margin</span><span class="sxs-lookup"><span data-stu-id="6e60e-122">margin</span></span>        | <span data-ttu-id="6e60e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6e60e-123">Int32</span></span>  | <span data-ttu-id="6e60e-124">A margem do cabeçalho na parte superior do documento.</span><span class="sxs-lookup"><span data-stu-id="6e60e-124">The margin of the header from the top of the document.</span></span>        |
| <span data-ttu-id="6e60e-125">texto</span><span class="sxs-lookup"><span data-stu-id="6e60e-125">text</span></span>          | <span data-ttu-id="6e60e-126">String</span><span class="sxs-lookup"><span data-stu-id="6e60e-126">String</span></span> | <span data-ttu-id="6e60e-127">O conteúdo do próprio cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="6e60e-127">The contents of the header itself.</span></span>                            |
| <span data-ttu-id="6e60e-128">uiElementname</span><span class="sxs-lookup"><span data-stu-id="6e60e-128">uiElementName</span></span> | <span data-ttu-id="6e60e-129">String</span><span class="sxs-lookup"><span data-stu-id="6e60e-129">String</span></span> | <span data-ttu-id="6e60e-130">O nome do elemento de interface do usuário onde o cabeçalho deve ser colocado.</span><span class="sxs-lookup"><span data-stu-id="6e60e-130">The name of the UI element where the header should be placed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e60e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e60e-131">JSON representation</span></span>

<span data-ttu-id="6e60e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e60e-132">The following is a JSON representation of the resource.</span></span>

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