---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: e9ef87063959f320068933a17c1fa8b0a70859da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003825"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="3a1ff-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="3a1ff-103">sizeRange resource type</span></span>


<span data-ttu-id="3a1ff-104">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="3a1ff-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="3a1ff-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a1ff-105">Properties</span></span>
| <span data-ttu-id="3a1ff-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a1ff-106">Property</span></span>     | <span data-ttu-id="3a1ff-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a1ff-107">Type</span></span>   |<span data-ttu-id="3a1ff-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a1ff-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a1ff-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="3a1ff-109">maximumSize</span></span> | <span data-ttu-id="3a1ff-110">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1ff-110">Int32</span></span> | <span data-ttu-id="3a1ff-111">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="3a1ff-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="3a1ff-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="3a1ff-112">minimumSize</span></span> | <span data-ttu-id="3a1ff-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3a1ff-113">Int32</span></span> | <span data-ttu-id="3a1ff-114">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="3a1ff-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3a1ff-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a1ff-115">JSON representation</span></span>
<span data-ttu-id="3a1ff-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a1ff-116">Here is a JSON representation of the resource.</span></span>

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