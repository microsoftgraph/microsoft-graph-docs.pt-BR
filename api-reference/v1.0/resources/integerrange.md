---
title: Tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descrito por dois limites int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: aee4ebfab164e6abbbecde083ba028c4c5a98723
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516843"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="019fa-103">Tipo de recurso integerRange</span><span class="sxs-lookup"><span data-stu-id="019fa-103">integerRange resource type</span></span>

<span data-ttu-id="019fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="019fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="019fa-105">Representa um intervalo inclusivo de inteiros descrito por dois limites int64.</span><span class="sxs-lookup"><span data-stu-id="019fa-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="019fa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="019fa-106">Properties</span></span>
| <span data-ttu-id="019fa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="019fa-107">Property</span></span>     | <span data-ttu-id="019fa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="019fa-108">Type</span></span>        | <span data-ttu-id="019fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="019fa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="019fa-110">iniciar</span><span class="sxs-lookup"><span data-stu-id="019fa-110">start</span></span>|<span data-ttu-id="019fa-111">Int64</span><span class="sxs-lookup"><span data-stu-id="019fa-111">Int64</span></span>|<span data-ttu-id="019fa-112">O limite inferior inclusivo do intervalo inteiro.</span><span class="sxs-lookup"><span data-stu-id="019fa-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="019fa-113">end</span><span class="sxs-lookup"><span data-stu-id="019fa-113">end</span></span>|<span data-ttu-id="019fa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="019fa-114">Int64</span></span>|<span data-ttu-id="019fa-115">O limite superior inclusivo do intervalo inteiro.</span><span class="sxs-lookup"><span data-stu-id="019fa-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="019fa-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="019fa-116">JSON representation</span></span>

<span data-ttu-id="019fa-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="019fa-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```