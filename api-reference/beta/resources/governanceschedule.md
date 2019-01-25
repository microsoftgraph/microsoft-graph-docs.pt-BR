---
title: tipo de recurso de governanceSchedule
description: 'Representa o agendamento para um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função. '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508024"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="e904f-104">tipo de recurso de governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="e904f-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e904f-105">Representa o agendamento para um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e904f-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="e904f-106">Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e904f-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="e904f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e904f-107">Properties</span></span>
| <span data-ttu-id="e904f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e904f-108">Property</span></span>     | <span data-ttu-id="e904f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e904f-109">Type</span></span>   |<span data-ttu-id="e904f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e904f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e904f-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e904f-111">startDateTime</span></span>|<span data-ttu-id="e904f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e904f-112">DateTimeOffset</span></span>|<span data-ttu-id="e904f-113">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e904f-113">The start time of the role assignment.</span></span> <span data-ttu-id="e904f-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e904f-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e904f-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e904f-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e904f-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e904f-116">endDateTime</span></span>|<span data-ttu-id="e904f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e904f-117">DateTimeOffset</span></span>|<span data-ttu-id="e904f-118">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e904f-118">The end time of the role assignment.</span></span> <span data-ttu-id="e904f-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e904f-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e904f-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e904f-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e904f-121">*Observação: se o valor for `null`, isso indica que uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="e904f-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="e904f-122">type</span><span class="sxs-lookup"><span data-stu-id="e904f-122">type</span></span>|<span data-ttu-id="e904f-123">String</span><span class="sxs-lookup"><span data-stu-id="e904f-123">String</span></span>|<span data-ttu-id="e904f-124">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e904f-124">The role assignment schedule type.</span></span> <span data-ttu-id="e904f-125">Somente `Once` é suportado para agora.</span><span class="sxs-lookup"><span data-stu-id="e904f-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="e904f-126">duration</span><span class="sxs-lookup"><span data-stu-id="e904f-126">duration</span></span>|<span data-ttu-id="e904f-127">Duration</span><span class="sxs-lookup"><span data-stu-id="e904f-127">Duration</span></span>|<span data-ttu-id="e904f-128">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e904f-128">The duration of a role assignment.</span></span> <span data-ttu-id="e904f-129">Ela está no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="e904f-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e904f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e904f-130">JSON representation</span></span>

<span data-ttu-id="e904f-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e904f-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
