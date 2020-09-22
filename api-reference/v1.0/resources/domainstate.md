---
title: tipo de recurso domainstate
description: Representa o status de operações assíncronas agendadas em um domínio.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fe1d6db925960214c19be27e218b254b31ea3f75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018624"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="7b3b1-103">tipo de recurso domainstate</span><span class="sxs-lookup"><span data-stu-id="7b3b1-103">domainState resource type</span></span>

<span data-ttu-id="7b3b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b3b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b3b1-105">Representa o status de operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="7b3b1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b3b1-106">Properties</span></span>

| <span data-ttu-id="7b3b1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b3b1-107">Property</span></span>   | <span data-ttu-id="7b3b1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b3b1-108">Type</span></span> | <span data-ttu-id="7b3b1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b3b1-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="7b3b1-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7b3b1-110">lastActionDateTime</span></span> | <span data-ttu-id="7b3b1-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b3b1-111">DateTimeOffset</span></span> | <span data-ttu-id="7b3b1-112">Carimbo de data/hora de quando a última atividade ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="7b3b1-113">O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="7b3b1-114">operações</span><span class="sxs-lookup"><span data-stu-id="7b3b1-114">operation</span></span> | <span data-ttu-id="7b3b1-115">String</span><span class="sxs-lookup"><span data-stu-id="7b3b1-115">String</span></span> | <span data-ttu-id="7b3b1-116">Tipo de operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-116">Type of asynchronous operation.</span></span> <span data-ttu-id="7b3b1-117">Os valores podem ser *ForceDelete* ou *verificação*</span><span class="sxs-lookup"><span data-stu-id="7b3b1-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="7b3b1-118">status</span><span class="sxs-lookup"><span data-stu-id="7b3b1-118">status</span></span> | <span data-ttu-id="7b3b1-119">String</span><span class="sxs-lookup"><span data-stu-id="7b3b1-119">String</span></span> | <span data-ttu-id="7b3b1-120">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-120">Current status of the operation.</span></span> <br> <span data-ttu-id="7b3b1-121">*Scheduled* -a operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="7b3b1-122">*InProgress* – a tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="7b3b1-123">*Failed* -a operação falhou.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b3b1-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b3b1-124">JSON representation</span></span>
<span data-ttu-id="7b3b1-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b3b1-125">Here is a JSON representation of the resource.</span></span>

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

