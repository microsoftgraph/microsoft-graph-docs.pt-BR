---
title: tipo de recurso governanceSchedule
description: 'Representa o agendamento de um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função. '
localization_priority: Normal
ms.openlocfilehash: 798b2a7f3e67ac466189f1ece55437214931056d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340279"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="3a929-104">tipo de recurso governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="3a929-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a929-105">Representa o agendamento de um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="3a929-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="3a929-106">Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3a929-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="3a929-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a929-107">Properties</span></span>
| <span data-ttu-id="3a929-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a929-108">Property</span></span>     | <span data-ttu-id="3a929-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a929-109">Type</span></span>   |<span data-ttu-id="3a929-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a929-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a929-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3a929-111">startDateTime</span></span>|<span data-ttu-id="3a929-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a929-112">DateTimeOffset</span></span>|<span data-ttu-id="3a929-113">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3a929-113">The start time of the role assignment.</span></span> <span data-ttu-id="3a929-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3a929-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3a929-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3a929-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3a929-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3a929-116">endDateTime</span></span>|<span data-ttu-id="3a929-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a929-117">DateTimeOffset</span></span>|<span data-ttu-id="3a929-118">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3a929-118">The end time of the role assignment.</span></span> <span data-ttu-id="3a929-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3a929-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3a929-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3a929-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3a929-121">*Observação: se o valor for `null`, ele indica uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="3a929-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="3a929-122">type</span><span class="sxs-lookup"><span data-stu-id="3a929-122">type</span></span>|<span data-ttu-id="3a929-123">String</span><span class="sxs-lookup"><span data-stu-id="3a929-123">String</span></span>|<span data-ttu-id="3a929-124">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3a929-124">The role assignment schedule type.</span></span> <span data-ttu-id="3a929-125">O `Once` só é suportado por enquanto.</span><span class="sxs-lookup"><span data-stu-id="3a929-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="3a929-126">duration</span><span class="sxs-lookup"><span data-stu-id="3a929-126">duration</span></span>|<span data-ttu-id="3a929-127">Duração</span><span class="sxs-lookup"><span data-stu-id="3a929-127">Duration</span></span>|<span data-ttu-id="3a929-128">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="3a929-128">The duration of a role assignment.</span></span> <span data-ttu-id="3a929-129">É no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="3a929-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a929-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a929-130">JSON representation</span></span>

<span data-ttu-id="3a929-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a929-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
