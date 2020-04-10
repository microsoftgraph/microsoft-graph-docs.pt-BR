---
title: tipo de recurso synchronizationSchedule
description: Define o agendamento usado para executar um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0f72c292954c7a5e7ae0d4c9d68a5ae900942f4d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217336"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="09b3c-103">tipo de recurso synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="09b3c-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="09b3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09b3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09b3c-105">Define o agendamento usado para executar um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="09b3c-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="09b3c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09b3c-106">Properties</span></span>
| <span data-ttu-id="09b3c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09b3c-107">Property</span></span>     | <span data-ttu-id="09b3c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="09b3c-108">Type</span></span>   |<span data-ttu-id="09b3c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b3c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09b3c-110">validade</span><span class="sxs-lookup"><span data-stu-id="09b3c-110">expiration</span></span>|<span data-ttu-id="09b3c-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b3c-111">DateTimeOffset</span></span>|<span data-ttu-id="09b3c-112">Data e hora em que este trabalho vai expirar.</span><span class="sxs-lookup"><span data-stu-id="09b3c-112">Date and time when this job will expire.</span></span> <span data-ttu-id="09b3c-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="09b3c-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="09b3c-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="09b3c-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="09b3c-115">interval</span><span class="sxs-lookup"><span data-stu-id="09b3c-115">interval</span></span>|<span data-ttu-id="09b3c-116">Duração</span><span class="sxs-lookup"><span data-stu-id="09b3c-116">Duration</span></span>|<span data-ttu-id="09b3c-117">O intervalo entre as iterações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="09b3c-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="09b3c-118">state</span><span class="sxs-lookup"><span data-stu-id="09b3c-118">state</span></span>|<span data-ttu-id="09b3c-119">String</span><span class="sxs-lookup"><span data-stu-id="09b3c-119">String</span></span>| <span data-ttu-id="09b3c-120">Os valores possíveis são: `Active` e `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="09b3c-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09b3c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09b3c-121">JSON representation</span></span>

<span data-ttu-id="09b3c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09b3c-122">The following is a JSON representation of the resource.</span></span>

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
