---
title: tipo de recurso genericError
description: Um erro de uso geral.
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333660"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="feebf-103">tipo de recurso genericError</span><span class="sxs-lookup"><span data-stu-id="feebf-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feebf-104">Um erro de uso geral.</span><span class="sxs-lookup"><span data-stu-id="feebf-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="feebf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feebf-105">Properties</span></span>

| <span data-ttu-id="feebf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feebf-106">Property</span></span> | <span data-ttu-id="feebf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="feebf-107">Type</span></span> | <span data-ttu-id="feebf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="feebf-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="feebf-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="feebf-109">message</span></span> | <span data-ttu-id="feebf-110">String</span><span class="sxs-lookup"><span data-stu-id="feebf-110">String</span></span> | <span data-ttu-id="feebf-111">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="feebf-111">The error message.</span></span> |
| <span data-ttu-id="feebf-112">código</span><span class="sxs-lookup"><span data-stu-id="feebf-112">code</span></span> | <span data-ttu-id="feebf-113">String</span><span class="sxs-lookup"><span data-stu-id="feebf-113">String</span></span> | <span data-ttu-id="feebf-114">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="feebf-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="feebf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feebf-115">JSON representation</span></span>

<span data-ttu-id="feebf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feebf-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
