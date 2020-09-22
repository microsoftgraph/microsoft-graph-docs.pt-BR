---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21a49f360ac18ad42ce5530a8cfcbcbea1876bc0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072855"
---
# <a name="operation-resource-type"></a><span data-ttu-id="ff356-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="ff356-103">operation resource type</span></span>

<span data-ttu-id="ff356-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff356-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff356-105">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="ff356-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff356-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff356-106">JSON representation</span></span>

<span data-ttu-id="ff356-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff356-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ff356-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff356-108">Properties</span></span>
| <span data-ttu-id="ff356-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff356-109">Property</span></span>     | <span data-ttu-id="ff356-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff356-110">Type</span></span>   |<span data-ttu-id="ff356-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff356-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff356-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff356-112">createdDateTime</span></span>| <span data-ttu-id="ff356-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff356-113">DateTimeOffset</span></span> |<span data-ttu-id="ff356-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="ff356-114">The start time of the operation.</span></span>|
|<span data-ttu-id="ff356-115">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="ff356-115">lastActionDateTime</span></span>| <span data-ttu-id="ff356-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff356-116">DateTimeOffset</span></span> |<span data-ttu-id="ff356-117">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="ff356-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="ff356-118">status</span><span class="sxs-lookup"><span data-stu-id="ff356-118">status</span></span>|<span data-ttu-id="ff356-119">operationStatus</span><span class="sxs-lookup"><span data-stu-id="ff356-119">operationStatus</span></span>|<span data-ttu-id="ff356-120">O status atual da operação: `notStarted` , `running` , `completed` , `failed`</span><span class="sxs-lookup"><span data-stu-id="ff356-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

