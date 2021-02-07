---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7eed9cfdd4739ee35c340d0cfeaeb8cc6d088455
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137078"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="67e4f-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="67e4f-103">sizeRange resource type</span></span>

<span data-ttu-id="67e4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e4f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="67e4f-105">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="67e4f-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="67e4f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67e4f-106">Properties</span></span>
| <span data-ttu-id="67e4f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67e4f-107">Property</span></span>     | <span data-ttu-id="67e4f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="67e4f-108">Type</span></span>   |<span data-ttu-id="67e4f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="67e4f-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="67e4f-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="67e4f-110">maximumSize</span></span> | <span data-ttu-id="67e4f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="67e4f-111">Int32</span></span> | <span data-ttu-id="67e4f-112">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="67e4f-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="67e4f-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="67e4f-113">minimumSize</span></span> | <span data-ttu-id="67e4f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="67e4f-114">Int32</span></span> | <span data-ttu-id="67e4f-115">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="67e4f-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="67e4f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67e4f-116">JSON representation</span></span>
<span data-ttu-id="67e4f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67e4f-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

