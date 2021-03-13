---
title: Tipo de recurso domainState
description: Representa o status de operações assíncronas agendadas em um domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 15189beb4441d606becc470f4fb3fbe14f4370c4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761111"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="b800e-103">Tipo de recurso domainState</span><span class="sxs-lookup"><span data-stu-id="b800e-103">domainState resource type</span></span>

<span data-ttu-id="b800e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b800e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b800e-105">Representa o status de operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="b800e-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="b800e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b800e-106">Properties</span></span>

| <span data-ttu-id="b800e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b800e-107">Property</span></span>   | <span data-ttu-id="b800e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b800e-108">Type</span></span> | <span data-ttu-id="b800e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b800e-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b800e-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b800e-110">lastActionDateTime</span></span> | <span data-ttu-id="b800e-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b800e-111">DateTimeOffset</span></span> | <span data-ttu-id="b800e-112">Timestamp para quando ocorreu a última atividade.</span><span class="sxs-lookup"><span data-stu-id="b800e-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="b800e-113">O valor é atualizado quando uma operação é agendada, a tarefa assíncrona é iniciada e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="b800e-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="b800e-114">operation</span><span class="sxs-lookup"><span data-stu-id="b800e-114">operation</span></span> | <span data-ttu-id="b800e-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b800e-115">String</span></span> | <span data-ttu-id="b800e-116">Tipo de operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="b800e-116">Type of asynchronous operation.</span></span> <span data-ttu-id="b800e-117">Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="b800e-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="b800e-118">status</span><span class="sxs-lookup"><span data-stu-id="b800e-118">status</span></span> | <span data-ttu-id="b800e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b800e-119">String</span></span> | <span data-ttu-id="b800e-120">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="b800e-120">Current status of the operation.</span></span> <br> <span data-ttu-id="b800e-121">*Agendado* - A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="b800e-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="b800e-122">*InProgress* - A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="b800e-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="b800e-123">*Falha* - Falha na operação.</span><span class="sxs-lookup"><span data-stu-id="b800e-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b800e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b800e-124">JSON representation</span></span>
<span data-ttu-id="b800e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b800e-125">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


