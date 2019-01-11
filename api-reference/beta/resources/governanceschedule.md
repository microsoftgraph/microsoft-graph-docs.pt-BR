---
title: tipo de recurso de governanceSchedule
description: 'Representa o agendamento para um governanceRoleAssignmentRequest. Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função. '
localization_priority: Normal
ms.openlocfilehash: 8bf36b786adbd8064ee0c00c0ce293408c6e2b7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882310"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="31083-104">tipo de recurso de governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="31083-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="31083-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31083-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31083-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31083-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31083-107">Representa o agendamento para um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="31083-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="31083-108">Para uma solicitação de atribuição de função, controla a agenda quando executar a operação de atribuição de função, quando parar de atribuição de função e a frequência de realizar a operação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="31083-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="31083-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31083-109">Properties</span></span>
| <span data-ttu-id="31083-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31083-110">Property</span></span>     | <span data-ttu-id="31083-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="31083-111">Type</span></span>   |<span data-ttu-id="31083-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="31083-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31083-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31083-113">startDateTime</span></span>|<span data-ttu-id="31083-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31083-114">DateTimeOffset</span></span>|<span data-ttu-id="31083-115">A hora de início da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="31083-115">The start time of the role assignment.</span></span> <span data-ttu-id="31083-116">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="31083-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31083-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="31083-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="31083-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="31083-118">endDateTime</span></span>|<span data-ttu-id="31083-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31083-119">DateTimeOffset</span></span>|<span data-ttu-id="31083-120">A hora de término da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="31083-120">The end time of the role assignment.</span></span> <span data-ttu-id="31083-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="31083-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31083-122">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31083-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="31083-123">*Observação: se o valor for `null`, isso indica que uma atribuição permanente.*</span><span class="sxs-lookup"><span data-stu-id="31083-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="31083-124">type</span><span class="sxs-lookup"><span data-stu-id="31083-124">type</span></span>|<span data-ttu-id="31083-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31083-125">String</span></span>|<span data-ttu-id="31083-126">O tipo de agendamento de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="31083-126">The role assignment schedule type.</span></span> <span data-ttu-id="31083-127">Somente `Once` é suportado para agora.</span><span class="sxs-lookup"><span data-stu-id="31083-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="31083-128">duration</span><span class="sxs-lookup"><span data-stu-id="31083-128">duration</span></span>|<span data-ttu-id="31083-129">Duração</span><span class="sxs-lookup"><span data-stu-id="31083-129">Duration</span></span>|<span data-ttu-id="31083-130">A duração de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="31083-130">The duration of a role assignment.</span></span> <span data-ttu-id="31083-131">Ela está no formato de um TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="31083-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31083-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31083-132">JSON representation</span></span>

<span data-ttu-id="31083-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31083-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
