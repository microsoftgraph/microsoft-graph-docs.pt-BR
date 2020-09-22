---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 54b66af210f6360938be1df964f14a089d8168fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090743"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="c58bd-103">tipo de recurso timeStamp</span><span class="sxs-lookup"><span data-stu-id="c58bd-103">timeStamp resource type</span></span>

<span data-ttu-id="c58bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c58bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c58bd-105">Informações de data e hora para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="c58bd-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c58bd-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c58bd-106">JSON representation</span></span>

<span data-ttu-id="c58bd-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c58bd-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c58bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c58bd-108">Properties</span></span>
| <span data-ttu-id="c58bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c58bd-109">Property</span></span>       | <span data-ttu-id="c58bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c58bd-110">Type</span></span>    |<span data-ttu-id="c58bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c58bd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c58bd-112">data</span><span class="sxs-lookup"><span data-stu-id="c58bd-112">date</span></span>|<span data-ttu-id="c58bd-113">Data</span><span class="sxs-lookup"><span data-stu-id="c58bd-113">Date</span></span>|<span data-ttu-id="c58bd-114">A parte de data do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="c58bd-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="c58bd-115">time</span><span class="sxs-lookup"><span data-stu-id="c58bd-115">time</span></span>|<span data-ttu-id="c58bd-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c58bd-116">TimeOfDay</span></span>|<span data-ttu-id="c58bd-117">A parte de tempo do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="c58bd-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="c58bd-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="c58bd-118">timeZone</span></span>|<span data-ttu-id="c58bd-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c58bd-119">String</span></span>|<span data-ttu-id="c58bd-120">A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.</span><span class="sxs-lookup"><span data-stu-id="c58bd-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

