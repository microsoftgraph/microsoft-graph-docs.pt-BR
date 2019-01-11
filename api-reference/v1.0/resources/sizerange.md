---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
ms.openlocfilehash: ae754d0666185023272860864ef17f038aecff7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873536"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="14131-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="14131-103">sizeRange resource type</span></span>


<span data-ttu-id="14131-104">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="14131-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="14131-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14131-105">Properties</span></span>
| <span data-ttu-id="14131-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14131-106">Property</span></span>     | <span data-ttu-id="14131-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="14131-107">Type</span></span>   |<span data-ttu-id="14131-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="14131-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14131-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="14131-109">maximumSize</span></span> | <span data-ttu-id="14131-110">Int32</span><span class="sxs-lookup"><span data-stu-id="14131-110">Int32</span></span> | <span data-ttu-id="14131-111">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="14131-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="14131-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="14131-112">minimumSize</span></span> | <span data-ttu-id="14131-113">Int32</span><span class="sxs-lookup"><span data-stu-id="14131-113">Int32</span></span> | <span data-ttu-id="14131-114">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="14131-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="14131-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14131-115">JSON representation</span></span>
<span data-ttu-id="14131-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14131-116">Here is a JSON representation of the resource.</span></span>

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
