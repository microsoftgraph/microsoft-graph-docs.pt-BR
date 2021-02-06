---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: af63282d3093fc0178dba6027846b2c080c3c5f9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136924"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="9722d-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="9722d-103">sizeRange resource type</span></span>

<span data-ttu-id="9722d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9722d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9722d-105">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="9722d-105">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="9722d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9722d-106">Properties</span></span>
| <span data-ttu-id="9722d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9722d-107">Property</span></span>     | <span data-ttu-id="9722d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9722d-108">Type</span></span>   |<span data-ttu-id="9722d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9722d-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9722d-110">maximumSize</span><span class="sxs-lookup"><span data-stu-id="9722d-110">maximumSize</span></span> | <span data-ttu-id="9722d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="9722d-111">Int32</span></span> | <span data-ttu-id="9722d-112">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="9722d-112">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="9722d-113">minimumSize</span><span class="sxs-lookup"><span data-stu-id="9722d-113">minimumSize</span></span> | <span data-ttu-id="9722d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9722d-114">Int32</span></span> | <span data-ttu-id="9722d-115">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="9722d-115">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9722d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9722d-116">JSON representation</span></span>
<span data-ttu-id="9722d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9722d-117">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


