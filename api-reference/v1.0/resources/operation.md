---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c9b920bbf696e80923c1d37756d7c27e1f06ab3a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808148"
---
# <a name="operation-resource-type"></a><span data-ttu-id="d698b-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="d698b-103">operation resource type</span></span>

<span data-ttu-id="d698b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d698b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d698b-105">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="d698b-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d698b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d698b-106">JSON representation</span></span>

<span data-ttu-id="d698b-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d698b-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d698b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d698b-108">Properties</span></span>
| <span data-ttu-id="d698b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d698b-109">Property</span></span>     | <span data-ttu-id="d698b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d698b-110">Type</span></span>   |<span data-ttu-id="d698b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d698b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d698b-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d698b-112">createdDateTime</span></span>| <span data-ttu-id="d698b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d698b-113">DateTimeOffset</span></span> |<span data-ttu-id="d698b-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="d698b-114">The start time of the operation.</span></span>|
|<span data-ttu-id="d698b-115">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d698b-115">lastActionDateTime</span></span>| <span data-ttu-id="d698b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d698b-116">DateTimeOffset</span></span> |<span data-ttu-id="d698b-117">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="d698b-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="d698b-118">status</span><span class="sxs-lookup"><span data-stu-id="d698b-118">status</span></span>|<span data-ttu-id="d698b-119">operationStatus</span><span class="sxs-lookup"><span data-stu-id="d698b-119">operationStatus</span></span>|<span data-ttu-id="d698b-120">O status atual da operação: `notStarted` , `running` , `completed` , `failed`</span><span class="sxs-lookup"><span data-stu-id="d698b-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
