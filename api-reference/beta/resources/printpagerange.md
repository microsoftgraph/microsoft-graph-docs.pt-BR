---
title: tipo de recurso printPageRange
description: Especifica o intervalo de páginas a serem impressas.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a8bbf452c337cb5c2ade7302eb29cff4bdb73d23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052534"
---
# <a name="printpagerange-resource-type"></a><span data-ttu-id="d29b7-103">tipo de recurso printPageRange</span><span class="sxs-lookup"><span data-stu-id="d29b7-103">printPageRange resource type</span></span>

<span data-ttu-id="d29b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d29b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29b7-105">Especifica o intervalo de páginas a serem impressas.</span><span class="sxs-lookup"><span data-stu-id="d29b7-105">Specifies the range of pages to be printed.</span></span>

## <a name="properties"></a><span data-ttu-id="d29b7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d29b7-106">Properties</span></span>
| <span data-ttu-id="d29b7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d29b7-107">Property</span></span>     | <span data-ttu-id="d29b7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d29b7-108">Type</span></span>        | <span data-ttu-id="d29b7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d29b7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d29b7-110">Inicial</span><span class="sxs-lookup"><span data-stu-id="d29b7-110">startPage</span></span>|<span data-ttu-id="d29b7-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d29b7-111">Int32</span></span>|<span data-ttu-id="d29b7-112">A página inicial (inclusive) do intervalo.</span><span class="sxs-lookup"><span data-stu-id="d29b7-112">The start page (inclusive) for the range.</span></span> <span data-ttu-id="d29b7-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d29b7-113">Read-only.</span></span>|
|<span data-ttu-id="d29b7-114">Página de fim</span><span class="sxs-lookup"><span data-stu-id="d29b7-114">endPage</span></span>|<span data-ttu-id="d29b7-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d29b7-115">Int32</span></span>|<span data-ttu-id="d29b7-116">A página final (inclusive) do intervalo.</span><span class="sxs-lookup"><span data-stu-id="d29b7-116">The end page (inclusive) for the range.</span></span> <span data-ttu-id="d29b7-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d29b7-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d29b7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d29b7-118">JSON representation</span></span>

<span data-ttu-id="d29b7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d29b7-119">The following is a JSON representation of the resource.</span></span>

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


