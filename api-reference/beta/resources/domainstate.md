---
title: tipo de recurso domainstate
description: Representa o status de operações assíncronas agendadas em um domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543158"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="7b430-103">tipo de recurso domainstate</span><span class="sxs-lookup"><span data-stu-id="7b430-103">domainState resource type</span></span>

<span data-ttu-id="7b430-104">Representa o status de operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="7b430-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="7b430-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b430-105">Properties</span></span>

| <span data-ttu-id="7b430-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b430-106">Property</span></span>   | <span data-ttu-id="7b430-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b430-107">Type</span></span> | <span data-ttu-id="7b430-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b430-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="7b430-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7b430-109">lastActionDateTime</span></span> | <span data-ttu-id="7b430-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b430-110">DateTimeOffset</span></span> | <span data-ttu-id="7b430-111">Carimbo de data/hora de quando a última atividade ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7b430-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="7b430-112">O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="7b430-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="7b430-113">operações</span><span class="sxs-lookup"><span data-stu-id="7b430-113">operation</span></span> | <span data-ttu-id="7b430-114">String</span><span class="sxs-lookup"><span data-stu-id="7b430-114">String</span></span> | <span data-ttu-id="7b430-115">Tipo de operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="7b430-115">Type of asynchronous operation.</span></span> <span data-ttu-id="7b430-116">Os valores podem ser *ForceDelete* ou *verificação*</span><span class="sxs-lookup"><span data-stu-id="7b430-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="7b430-117">status</span><span class="sxs-lookup"><span data-stu-id="7b430-117">status</span></span> | <span data-ttu-id="7b430-118">String</span><span class="sxs-lookup"><span data-stu-id="7b430-118">String</span></span> | <span data-ttu-id="7b430-119">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="7b430-119">Current status of the operation.</span></span> <br> <span data-ttu-id="7b430-120">*Scheduled* -a operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="7b430-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="7b430-121">*InProgress* – a tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="7b430-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="7b430-122">*Failed* -a operação falhou.</span><span class="sxs-lookup"><span data-stu-id="7b430-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b430-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b430-123">JSON representation</span></span>
<span data-ttu-id="7b430-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b430-124">Here is a JSON representation of the resource.</span></span>

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
