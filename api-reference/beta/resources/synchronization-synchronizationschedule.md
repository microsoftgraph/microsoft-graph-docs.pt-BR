---
title: Tipo de recurso synchronizationSchedule
description: Define o cronograma usado para executar um Trabalho de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 3d0b0a45515be459c436d24f8427f7b84ef1419f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722059"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="5b2b7-103">Tipo de recurso synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="5b2b7-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="5b2b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b2b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b2b7-105">Define o cronograma usado para executar uma [sincronizaçãoJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="5b2b7-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5b2b7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b2b7-106">Properties</span></span>
| <span data-ttu-id="5b2b7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b2b7-107">Property</span></span>     | <span data-ttu-id="5b2b7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b2b7-108">Type</span></span>   |<span data-ttu-id="5b2b7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b2b7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b2b7-110">expiration</span><span class="sxs-lookup"><span data-stu-id="5b2b7-110">expiration</span></span>|<span data-ttu-id="5b2b7-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b2b7-111">DateTimeOffset</span></span>|<span data-ttu-id="5b2b7-112">Data e hora em que esse trabalho expirará.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-112">Date and time when this job will expire.</span></span> <span data-ttu-id="5b2b7-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b2b7-114">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5b2b7-115">interval</span><span class="sxs-lookup"><span data-stu-id="5b2b7-115">interval</span></span>|<span data-ttu-id="5b2b7-116">Duration</span><span class="sxs-lookup"><span data-stu-id="5b2b7-116">Duration</span></span>|<span data-ttu-id="5b2b7-117">O intervalo entre iterações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="5b2b7-118">estado</span><span class="sxs-lookup"><span data-stu-id="5b2b7-118">state</span></span>|<span data-ttu-id="5b2b7-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b2b7-119">String</span></span>| <span data-ttu-id="5b2b7-120">Os valores possíveis são: `Active` e `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b2b7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b2b7-121">JSON representation</span></span>

<span data-ttu-id="5b2b7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b2b7-122">The following is a JSON representation of the resource.</span></span>

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


