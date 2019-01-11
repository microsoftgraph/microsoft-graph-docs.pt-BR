---
title: Tipo de recurso domainState
description: Representa o status das operações assíncronas agendadas em um domínio.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 3701e80c5104c80eae0cdfb4b1b9f549177a2cbf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830216"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="4d8e8-103">Tipo de recurso domainState</span><span class="sxs-lookup"><span data-stu-id="4d8e8-103">domainState resource type</span></span>

> <span data-ttu-id="4d8e8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d8e8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d8e8-106">Representa o status das operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="4d8e8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d8e8-107">Properties</span></span>

| <span data-ttu-id="4d8e8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d8e8-108">Property</span></span>   | <span data-ttu-id="4d8e8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d8e8-109">Type</span></span> | <span data-ttu-id="4d8e8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d8e8-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4d8e8-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4d8e8-111">lastActionDateTime</span></span> | <span data-ttu-id="4d8e8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d8e8-112">DateTimeOffset</span></span> | <span data-ttu-id="4d8e8-p102">O carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona começa e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="4d8e8-115">operação</span><span class="sxs-lookup"><span data-stu-id="4d8e8-115">operation</span></span> | <span data-ttu-id="4d8e8-116">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-116">String</span></span> | <span data-ttu-id="4d8e8-p103">Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="4d8e8-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="4d8e8-119">status</span><span class="sxs-lookup"><span data-stu-id="4d8e8-119">status</span></span> | <span data-ttu-id="4d8e8-120">String</span><span class="sxs-lookup"><span data-stu-id="4d8e8-120">String</span></span> | <span data-ttu-id="4d8e8-121">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-121">Current status of the operation.</span></span> <br> <span data-ttu-id="4d8e8-122">*Scheduled* – A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="4d8e8-123">*InProgress* – A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="4d8e8-124">*Failed* - A operação falhou.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d8e8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d8e8-125">JSON representation</span></span>
<span data-ttu-id="4d8e8-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d8e8-126">Here is a JSON representation of the resource.</span></span>

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
