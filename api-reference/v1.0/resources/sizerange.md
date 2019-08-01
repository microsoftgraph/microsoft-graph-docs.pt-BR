---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e9c174216508679373c607dc9a2acd95df9096c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034143"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="51a23-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="51a23-103">sizeRange resource type</span></span>


<span data-ttu-id="51a23-104">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="51a23-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="51a23-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51a23-105">Properties</span></span>
| <span data-ttu-id="51a23-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51a23-106">Property</span></span>     | <span data-ttu-id="51a23-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a23-107">Type</span></span>   |<span data-ttu-id="51a23-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a23-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51a23-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="51a23-109">maximumSize</span></span> | <span data-ttu-id="51a23-110">Int32</span><span class="sxs-lookup"><span data-stu-id="51a23-110">Int32</span></span> | <span data-ttu-id="51a23-111">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="51a23-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="51a23-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="51a23-112">minimumSize</span></span> | <span data-ttu-id="51a23-113">Int32</span><span class="sxs-lookup"><span data-stu-id="51a23-113">Int32</span></span> | <span data-ttu-id="51a23-114">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="51a23-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="51a23-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51a23-115">JSON representation</span></span>
<span data-ttu-id="51a23-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51a23-116">Here is a JSON representation of the resource.</span></span>

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
