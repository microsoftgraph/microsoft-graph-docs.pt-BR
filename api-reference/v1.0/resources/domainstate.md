---
title: Tipo de recurso domainState
description: Representa o status de operações assíncronas agendadas em um domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9ab9a4af3109e35cd1022b4d62869ce3bb034100
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761181"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="abbb6-103">Tipo de recurso domainState</span><span class="sxs-lookup"><span data-stu-id="abbb6-103">domainState resource type</span></span>

<span data-ttu-id="abbb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abbb6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abbb6-105">Representa o status de operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="abbb6-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="abbb6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abbb6-106">Properties</span></span>

| <span data-ttu-id="abbb6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abbb6-107">Property</span></span>   | <span data-ttu-id="abbb6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="abbb6-108">Type</span></span> | <span data-ttu-id="abbb6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="abbb6-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="abbb6-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="abbb6-110">lastActionDateTime</span></span> | <span data-ttu-id="abbb6-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbb6-111">DateTimeOffset</span></span> | <span data-ttu-id="abbb6-112">Timestamp para quando ocorreu a última atividade.</span><span class="sxs-lookup"><span data-stu-id="abbb6-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="abbb6-113">O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="abbb6-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="abbb6-114">operation</span><span class="sxs-lookup"><span data-stu-id="abbb6-114">operation</span></span> | <span data-ttu-id="abbb6-115">String</span><span class="sxs-lookup"><span data-stu-id="abbb6-115">String</span></span> | <span data-ttu-id="abbb6-116">Tipo de operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="abbb6-116">Type of asynchronous operation.</span></span> <span data-ttu-id="abbb6-117">Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="abbb6-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="abbb6-118">status</span><span class="sxs-lookup"><span data-stu-id="abbb6-118">status</span></span> | <span data-ttu-id="abbb6-119">String</span><span class="sxs-lookup"><span data-stu-id="abbb6-119">String</span></span> | <span data-ttu-id="abbb6-120">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="abbb6-120">Current status of the operation.</span></span> <br> <span data-ttu-id="abbb6-121">*Agendado* - A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="abbb6-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="abbb6-122">*InProgress* - A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="abbb6-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="abbb6-123">*Falha* - Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="abbb6-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="abbb6-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abbb6-124">JSON representation</span></span>
<span data-ttu-id="abbb6-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abbb6-125">Here is a JSON representation of the resource.</span></span>

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

