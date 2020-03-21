---
title: tipo de recurso printPageRange
description: Especifica o intervalo de páginas a serem impressas.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 65e2455438dbdb8c7bef3ef3439f846e737ebba0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895472"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="1bee8-103">tipo de recurso printPageRange</span><span class="sxs-lookup"><span data-stu-id="1bee8-103">printPageRange resource type</span></span>

<span data-ttu-id="1bee8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bee8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bee8-105">Especifica o intervalo de páginas a serem impressas.</span><span class="sxs-lookup"><span data-stu-id="1bee8-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="1bee8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bee8-106">Properties</span></span>
| <span data-ttu-id="1bee8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bee8-107">Property</span></span>     | <span data-ttu-id="1bee8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bee8-108">Type</span></span>        | <span data-ttu-id="1bee8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bee8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1bee8-110">Inicial</span><span class="sxs-lookup"><span data-stu-id="1bee8-110">startPage</span></span>|<span data-ttu-id="1bee8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="1bee8-111">Int32</span></span>|<span data-ttu-id="1bee8-112">A página inicial (inclusive) do intervalo.</span><span class="sxs-lookup"><span data-stu-id="1bee8-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="1bee8-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1bee8-113">Read-only.</span></span>|
|<span data-ttu-id="1bee8-114">Página de fim</span><span class="sxs-lookup"><span data-stu-id="1bee8-114">endPage</span></span>|<span data-ttu-id="1bee8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1bee8-115">Int32</span></span>|<span data-ttu-id="1bee8-116">A página final (inclusive) do intervalo.</span><span class="sxs-lookup"><span data-stu-id="1bee8-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="1bee8-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1bee8-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1bee8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bee8-118">JSON representation</span></span>

<span data-ttu-id="1bee8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bee8-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": 123456,
  "endPage": 123456
}
```
