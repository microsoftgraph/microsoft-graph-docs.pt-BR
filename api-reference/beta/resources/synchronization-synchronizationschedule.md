---
title: tipo de recurso de synchronizationSchedule
description: Define a agenda usada para executar um synchronizationJob.
ms.openlocfilehash: c0435b3957f138751f34a1e0e522683b352294da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036898"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="273ab-103">tipo de recurso de synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="273ab-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="273ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="273ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="273ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="273ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="273ab-106">Define a agenda usada para executar um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="273ab-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="273ab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="273ab-107">Properties</span></span>
| <span data-ttu-id="273ab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="273ab-108">Property</span></span>     | <span data-ttu-id="273ab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="273ab-109">Type</span></span>   |<span data-ttu-id="273ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="273ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="273ab-111">expiração</span><span class="sxs-lookup"><span data-stu-id="273ab-111">expiration</span></span>|<span data-ttu-id="273ab-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="273ab-112">DateTimeOffset</span></span>|<span data-ttu-id="273ab-113">Data e hora em que esse trabalho expirará.</span><span class="sxs-lookup"><span data-stu-id="273ab-113">Date and time when this job will expire.</span></span> <span data-ttu-id="273ab-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="273ab-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="273ab-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="273ab-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="273ab-116">interval</span><span class="sxs-lookup"><span data-stu-id="273ab-116">interval</span></span>|<span data-ttu-id="273ab-117">Duração</span><span class="sxs-lookup"><span data-stu-id="273ab-117">Duration</span></span>|<span data-ttu-id="273ab-118">O intervalo entre iterações de sincronização.</span><span class="sxs-lookup"><span data-stu-id="273ab-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="273ab-119">state</span><span class="sxs-lookup"><span data-stu-id="273ab-119">state</span></span>|<span data-ttu-id="273ab-120">String</span><span class="sxs-lookup"><span data-stu-id="273ab-120">String</span></span>| <span data-ttu-id="273ab-121">Os valores possíveis são: `Active` e `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="273ab-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="273ab-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="273ab-122">JSON representation</span></span>

<span data-ttu-id="273ab-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="273ab-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->