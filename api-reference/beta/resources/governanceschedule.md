---
title: Tipo de recurso governanceSchedule
description: 'Representa o cronograma de uma governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência executar a operação de atribuição de função. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e7b444b1daa45daf3228476fb48a38be4e7bb2b2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132661"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="fa9ec-104">Tipo de recurso governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="fa9ec-104">governanceSchedule resource type</span></span>

<span data-ttu-id="fa9ec-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa9ec-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa9ec-106">Representa o cronograma de uma [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fa9ec-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="fa9ec-107">Para uma solicitação de atribuição de função, o agendamento controla quando executar a operação de atribuição de função, quando interromper a atribuição de função e com que frequência executar a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="fa9ec-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa9ec-108">Properties</span></span>
| <span data-ttu-id="fa9ec-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa9ec-109">Property</span></span>     | <span data-ttu-id="fa9ec-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa9ec-110">Type</span></span>   |<span data-ttu-id="fa9ec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa9ec-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa9ec-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fa9ec-112">startDateTime</span></span>|<span data-ttu-id="fa9ec-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa9ec-113">DateTimeOffset</span></span>|<span data-ttu-id="fa9ec-114">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-114">The start time of the role assignment.</span></span> <span data-ttu-id="fa9ec-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa9ec-116">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fa9ec-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fa9ec-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fa9ec-117">endDateTime</span></span>|<span data-ttu-id="fa9ec-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa9ec-118">DateTimeOffset</span></span>|<span data-ttu-id="fa9ec-119">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-119">The end time of the role assignment.</span></span> <span data-ttu-id="fa9ec-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fa9ec-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fa9ec-122">*Observação: se o valor for `null` , ele indicará uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="fa9ec-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="fa9ec-123">type</span><span class="sxs-lookup"><span data-stu-id="fa9ec-123">type</span></span>|<span data-ttu-id="fa9ec-124">String</span><span class="sxs-lookup"><span data-stu-id="fa9ec-124">String</span></span>|<span data-ttu-id="fa9ec-125">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-125">The role assignment schedule type.</span></span> <span data-ttu-id="fa9ec-126">Só `Once` há suporte por enquanto.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="fa9ec-127">duração</span><span class="sxs-lookup"><span data-stu-id="fa9ec-127">duration</span></span>|<span data-ttu-id="fa9ec-128">Duration</span><span class="sxs-lookup"><span data-stu-id="fa9ec-128">Duration</span></span>|<span data-ttu-id="fa9ec-129">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-129">The duration of a role assignment.</span></span> <span data-ttu-id="fa9ec-130">Ele está no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa9ec-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa9ec-131">JSON representation</span></span>

<span data-ttu-id="fa9ec-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa9ec-132">Here is a JSON representation of the resource.</span></span>

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


