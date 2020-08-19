---
title: tipo de recurso governanceSchedule
description: 'Representa o agendamento de um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: b2a0a4ff42da594f9a74e26cc0facca9564548eb
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809499"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="d12ef-104">tipo de recurso governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="d12ef-104">governanceSchedule resource type</span></span>

<span data-ttu-id="d12ef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d12ef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d12ef-106">Representa o agendamento de um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="d12ef-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="d12ef-107">Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando parar a atribuição de função e com que frequência realizar a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d12ef-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="d12ef-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d12ef-108">Properties</span></span>
| <span data-ttu-id="d12ef-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d12ef-109">Property</span></span>     | <span data-ttu-id="d12ef-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d12ef-110">Type</span></span>   |<span data-ttu-id="d12ef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d12ef-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d12ef-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d12ef-112">startDateTime</span></span>|<span data-ttu-id="d12ef-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d12ef-113">DateTimeOffset</span></span>|<span data-ttu-id="d12ef-114">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d12ef-114">The start time of the role assignment.</span></span> <span data-ttu-id="d12ef-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d12ef-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d12ef-116">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d12ef-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d12ef-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d12ef-117">endDateTime</span></span>|<span data-ttu-id="d12ef-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d12ef-118">DateTimeOffset</span></span>|<span data-ttu-id="d12ef-119">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d12ef-119">The end time of the role assignment.</span></span> <span data-ttu-id="d12ef-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d12ef-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d12ef-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d12ef-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d12ef-122">*Observação: se o valor for `null` , ele indica uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="d12ef-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="d12ef-123">type</span><span class="sxs-lookup"><span data-stu-id="d12ef-123">type</span></span>|<span data-ttu-id="d12ef-124">String</span><span class="sxs-lookup"><span data-stu-id="d12ef-124">String</span></span>|<span data-ttu-id="d12ef-125">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d12ef-125">The role assignment schedule type.</span></span> <span data-ttu-id="d12ef-126">O só `Once` é suportado por enquanto.</span><span class="sxs-lookup"><span data-stu-id="d12ef-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="d12ef-127">duration</span><span class="sxs-lookup"><span data-stu-id="d12ef-127">duration</span></span>|<span data-ttu-id="d12ef-128">Duração</span><span class="sxs-lookup"><span data-stu-id="d12ef-128">Duration</span></span>|<span data-ttu-id="d12ef-129">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d12ef-129">The duration of a role assignment.</span></span> <span data-ttu-id="d12ef-130">É no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="d12ef-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d12ef-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d12ef-131">JSON representation</span></span>

<span data-ttu-id="d12ef-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d12ef-132">Here is a JSON representation of the resource.</span></span>

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
