---
title: tipo de recurso de synchronizationSchedule
description: Define a agenda usada para executar um synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 0e9714e4833c5586e54c8d812a0d72e41a513e5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515584"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="d93a2-103">tipo de recurso de synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="d93a2-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d93a2-104">Define a agenda usada para executar um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="d93a2-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d93a2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d93a2-105">Properties</span></span>
| <span data-ttu-id="d93a2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d93a2-106">Property</span></span>     | <span data-ttu-id="d93a2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d93a2-107">Type</span></span>   |<span data-ttu-id="d93a2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d93a2-109">Expiração</span><span class="sxs-lookup"><span data-stu-id="d93a2-109">expiration</span></span>|<span data-ttu-id="d93a2-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d93a2-110">DateTimeOffset</span></span>|<span data-ttu-id="d93a2-111">Data e hora em que esse trabalho expirará.</span><span class="sxs-lookup"><span data-stu-id="d93a2-111">Date and time when this job will expire.</span></span> <span data-ttu-id="d93a2-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d93a2-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d93a2-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d93a2-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d93a2-114">interval</span><span class="sxs-lookup"><span data-stu-id="d93a2-114">interval</span></span>|<span data-ttu-id="d93a2-115">Duration</span><span class="sxs-lookup"><span data-stu-id="d93a2-115">Duration</span></span>|<span data-ttu-id="d93a2-116">O intervalo entre iterações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="d93a2-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="d93a2-117">estado</span><span class="sxs-lookup"><span data-stu-id="d93a2-117">state</span></span>|<span data-ttu-id="d93a2-118">String</span><span class="sxs-lookup"><span data-stu-id="d93a2-118">String</span></span>| <span data-ttu-id="d93a2-119">Os valores possíveis são: `Active` e `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="d93a2-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d93a2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d93a2-120">JSON representation</span></span>

<span data-ttu-id="d93a2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d93a2-121">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
