---
title: tipo de recurso de operação
description: O status de uma operação de execução longa.
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884963"
---
# <a name="operation-resource-type"></a><span data-ttu-id="f152e-103">tipo de recurso de operação</span><span class="sxs-lookup"><span data-stu-id="f152e-103">operation resource type</span></span>

<span data-ttu-id="f152e-104">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="f152e-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f152e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f152e-105">JSON representation</span></span>

<span data-ttu-id="f152e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f152e-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="f152e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f152e-107">Properties</span></span>
| <span data-ttu-id="f152e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f152e-108">Property</span></span>     | <span data-ttu-id="f152e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f152e-109">Type</span></span>   |<span data-ttu-id="f152e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f152e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f152e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f152e-111">createdDateTime</span></span>| <span data-ttu-id="f152e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f152e-112">DateTimeOffset</span></span> |<span data-ttu-id="f152e-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="f152e-113">The start time of the operation.</span></span>|
|<span data-ttu-id="f152e-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f152e-114">lastActionDateTime</span></span>| <span data-ttu-id="f152e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f152e-115">DateTimeOffset</span></span> |<span data-ttu-id="f152e-116">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="f152e-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f152e-117">status</span><span class="sxs-lookup"><span data-stu-id="f152e-117">status</span></span>|<span data-ttu-id="f152e-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="f152e-118">operationStatus</span></span>|<span data-ttu-id="f152e-119">O status atual da operação: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="f152e-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
