---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8088d704d5a075131d5ee1b2c3b9edf75785708b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035725"
---
# <a name="operation-resource-type"></a><span data-ttu-id="b1ebd-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="b1ebd-103">operation resource type</span></span>

<span data-ttu-id="b1ebd-104">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b1ebd-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1ebd-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1ebd-105">JSON representation</span></span>

<span data-ttu-id="b1ebd-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1ebd-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b1ebd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1ebd-107">Properties</span></span>
| <span data-ttu-id="b1ebd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1ebd-108">Property</span></span>     | <span data-ttu-id="b1ebd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1ebd-109">Type</span></span>   |<span data-ttu-id="b1ebd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1ebd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1ebd-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1ebd-111">createdDateTime</span></span>| <span data-ttu-id="b1ebd-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1ebd-112">DateTimeOffset</span></span> |<span data-ttu-id="b1ebd-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="b1ebd-113">The start time of the operation.</span></span>|
|<span data-ttu-id="b1ebd-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b1ebd-114">lastActionDateTime</span></span>| <span data-ttu-id="b1ebd-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1ebd-115">DateTimeOffset</span></span> |<span data-ttu-id="b1ebd-116">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="b1ebd-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="b1ebd-117">status</span><span class="sxs-lookup"><span data-stu-id="b1ebd-117">status</span></span>|<span data-ttu-id="b1ebd-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="b1ebd-118">operationStatus</span></span>|<span data-ttu-id="b1ebd-119">O status atual da operação: `notStarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="b1ebd-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
