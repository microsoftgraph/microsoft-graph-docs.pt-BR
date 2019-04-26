---
title: tipo de recurso synchronizationSchedule
description: Define o agendamento usado para executar um synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 2ae5473463e84fdf27882df1b243049cc98ab043
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340029"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="9d433-103">tipo de recurso synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="9d433-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d433-104">Define o agendamento usado para executar um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="9d433-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9d433-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d433-105">Properties</span></span>
| <span data-ttu-id="9d433-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d433-106">Property</span></span>     | <span data-ttu-id="9d433-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d433-107">Type</span></span>   |<span data-ttu-id="9d433-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d433-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d433-109">validade</span><span class="sxs-lookup"><span data-stu-id="9d433-109">expiration</span></span>|<span data-ttu-id="9d433-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d433-110">DateTimeOffset</span></span>|<span data-ttu-id="9d433-111">Data e hora em que este trabalho vai expirar.</span><span class="sxs-lookup"><span data-stu-id="9d433-111">Date and time when this job will expire.</span></span> <span data-ttu-id="9d433-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9d433-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9d433-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9d433-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9d433-114">interval</span><span class="sxs-lookup"><span data-stu-id="9d433-114">interval</span></span>|<span data-ttu-id="9d433-115">Duração</span><span class="sxs-lookup"><span data-stu-id="9d433-115">Duration</span></span>|<span data-ttu-id="9d433-116">O intervalo entre as iterações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9d433-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="9d433-117">state</span><span class="sxs-lookup"><span data-stu-id="9d433-117">state</span></span>|<span data-ttu-id="9d433-118">String</span><span class="sxs-lookup"><span data-stu-id="9d433-118">String</span></span>| <span data-ttu-id="9d433-119">Os valores possíveis são: `Active` e `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="9d433-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d433-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d433-120">JSON representation</span></span>

<span data-ttu-id="9d433-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d433-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
