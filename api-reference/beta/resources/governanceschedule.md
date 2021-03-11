---
title: Tipo de recurso governanceSchedule
description: 'Representa a agenda de um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência fará a operação de atribuição de função. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f7583f15641c541493ded9f9a4779777e9f35f2a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722276"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="24bf3-104">Tipo de recurso governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="24bf3-104">governanceSchedule resource type</span></span>

<span data-ttu-id="24bf3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24bf3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24bf3-106">Representa a agenda de [um governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="24bf3-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="24bf3-107">Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência fará a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="24bf3-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="24bf3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24bf3-108">Properties</span></span>
| <span data-ttu-id="24bf3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24bf3-109">Property</span></span>     | <span data-ttu-id="24bf3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="24bf3-110">Type</span></span>   |<span data-ttu-id="24bf3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="24bf3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24bf3-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="24bf3-112">startDateTime</span></span>|<span data-ttu-id="24bf3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24bf3-113">DateTimeOffset</span></span>|<span data-ttu-id="24bf3-114">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="24bf3-114">The start time of the role assignment.</span></span> <span data-ttu-id="24bf3-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24bf3-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24bf3-116">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="24bf3-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="24bf3-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="24bf3-117">endDateTime</span></span>|<span data-ttu-id="24bf3-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24bf3-118">DateTimeOffset</span></span>|<span data-ttu-id="24bf3-119">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="24bf3-119">The end time of the role assignment.</span></span> <span data-ttu-id="24bf3-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24bf3-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24bf3-121">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="24bf3-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="24bf3-122">*Observação: se o valor for `null` , ele indicará uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="24bf3-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="24bf3-123">tipo</span><span class="sxs-lookup"><span data-stu-id="24bf3-123">type</span></span>|<span data-ttu-id="24bf3-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24bf3-124">String</span></span>|<span data-ttu-id="24bf3-125">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="24bf3-125">The role assignment schedule type.</span></span> <span data-ttu-id="24bf3-126">Por `Once` enquanto, só há suporte.</span><span class="sxs-lookup"><span data-stu-id="24bf3-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="24bf3-127">duração</span><span class="sxs-lookup"><span data-stu-id="24bf3-127">duration</span></span>|<span data-ttu-id="24bf3-128">Duration</span><span class="sxs-lookup"><span data-stu-id="24bf3-128">Duration</span></span>|<span data-ttu-id="24bf3-129">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="24bf3-129">The duration of a role assignment.</span></span> <span data-ttu-id="24bf3-130">Está no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="24bf3-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24bf3-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24bf3-131">JSON representation</span></span>

<span data-ttu-id="24bf3-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24bf3-132">Here is a JSON representation of the resource.</span></span>

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


