---
title: Tipo de recurso domainState
description: Representa o status das operações assíncronas agendadas em um domínio.
author: lleonard-msft
ms.openlocfilehash: 08484f29202ab348e2eca443a95f63ffbe645220
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351671"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="e53f9-103">Tipo de recurso domainState</span><span class="sxs-lookup"><span data-stu-id="e53f9-103">domainState resource type</span></span>

<span data-ttu-id="e53f9-104">Representa o status das operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="e53f9-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="e53f9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e53f9-105">Properties</span></span>

| <span data-ttu-id="e53f9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e53f9-106">Property</span></span>   | <span data-ttu-id="e53f9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e53f9-107">Type</span></span> | <span data-ttu-id="e53f9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e53f9-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e53f9-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e53f9-109">lastActionDateTime</span></span> | <span data-ttu-id="e53f9-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53f9-110">DateTimeOffset</span></span> | <span data-ttu-id="e53f9-p101">O carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona começa e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="e53f9-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="e53f9-113">operação</span><span class="sxs-lookup"><span data-stu-id="e53f9-113">operation</span></span> | <span data-ttu-id="e53f9-114">String</span><span class="sxs-lookup"><span data-stu-id="e53f9-114">String</span></span> | <span data-ttu-id="e53f9-p102">Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="e53f9-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="e53f9-117">status</span><span class="sxs-lookup"><span data-stu-id="e53f9-117">status</span></span> | <span data-ttu-id="e53f9-118">String</span><span class="sxs-lookup"><span data-stu-id="e53f9-118">String</span></span> | <span data-ttu-id="e53f9-119">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="e53f9-119">Current status of the operation.</span></span> <br> <span data-ttu-id="e53f9-120">*Scheduled* – A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="e53f9-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="e53f9-121">*InProgress* – A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="e53f9-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="e53f9-122">*Failed* - A operação falhou.</span><span class="sxs-lookup"><span data-stu-id="e53f9-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e53f9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e53f9-123">JSON representation</span></span>
<span data-ttu-id="e53f9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e53f9-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->