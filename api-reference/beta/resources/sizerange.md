---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
localization_priority: Normal
ms.openlocfilehash: c2a37c91c968eddffc4aca0c8cf783e5aac1f3eb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343000"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="f46db-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="f46db-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46db-104">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f46db-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="f46db-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f46db-105">Properties</span></span>
| <span data-ttu-id="f46db-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f46db-106">Property</span></span>     | <span data-ttu-id="f46db-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f46db-107">Type</span></span>   |<span data-ttu-id="f46db-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46db-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f46db-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="f46db-109">maximumSize</span></span> | <span data-ttu-id="f46db-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f46db-110">Int32</span></span> | <span data-ttu-id="f46db-111">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f46db-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="f46db-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="f46db-112">minimumSize</span></span> | <span data-ttu-id="f46db-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f46db-113">Int32</span></span> | <span data-ttu-id="f46db-114">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f46db-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f46db-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f46db-115">JSON representation</span></span>
<span data-ttu-id="f46db-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f46db-116">Here is a JSON representation of the resource.</span></span>

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
