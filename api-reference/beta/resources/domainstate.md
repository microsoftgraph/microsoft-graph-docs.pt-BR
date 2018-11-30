---
title: Tipo de recurso domainState
description: Representa o status das operações assíncronas agendadas em um domínio.
ms.openlocfilehash: 84c2e418a14de8aa05abfac7a2f04d6637d410b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033855"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="8e7a0-103">Tipo de recurso domainState</span><span class="sxs-lookup"><span data-stu-id="8e7a0-103">domainState resource type</span></span>

> <span data-ttu-id="8e7a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e7a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e7a0-106">Representa o status das operações assíncronas agendadas em um domínio.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="8e7a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e7a0-107">Properties</span></span>

| <span data-ttu-id="8e7a0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e7a0-108">Property</span></span>   | <span data-ttu-id="8e7a0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e7a0-109">Type</span></span> | <span data-ttu-id="8e7a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e7a0-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8e7a0-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7a0-111">lastActionDateTime</span></span> | <span data-ttu-id="8e7a0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7a0-112">DateTimeOffset</span></span> | <span data-ttu-id="8e7a0-p102">O carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona começa e quando a operação é concluída.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="8e7a0-115">operação</span><span class="sxs-lookup"><span data-stu-id="8e7a0-115">operation</span></span> | <span data-ttu-id="8e7a0-116">String</span><span class="sxs-lookup"><span data-stu-id="8e7a0-116">String</span></span> | <span data-ttu-id="8e7a0-p103">Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification*</span><span class="sxs-lookup"><span data-stu-id="8e7a0-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="8e7a0-119">status</span><span class="sxs-lookup"><span data-stu-id="8e7a0-119">status</span></span> | <span data-ttu-id="8e7a0-120">String</span><span class="sxs-lookup"><span data-stu-id="8e7a0-120">String</span></span> | <span data-ttu-id="8e7a0-121">Status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-121">Current status of the operation.</span></span> <br> <span data-ttu-id="8e7a0-122">*Scheduled* – A operação foi agendada, mas não foi iniciada.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="8e7a0-123">*InProgress* – A tarefa foi iniciada e está em andamento.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="8e7a0-124">*Failed* - A operação falhou.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e7a0-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e7a0-125">JSON representation</span></span>
<span data-ttu-id="8e7a0-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e7a0-126">Here is a JSON representation of the resource.</span></span>

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