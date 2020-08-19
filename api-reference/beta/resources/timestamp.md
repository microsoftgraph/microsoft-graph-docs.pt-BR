---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: JeremyKelley
ms.openlocfilehash: 1037212f1adb0fb10326bbdf88416877e16a9fbe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810990"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="ebe28-103">tipo de recurso timeStamp</span><span class="sxs-lookup"><span data-stu-id="ebe28-103">timeStamp resource type</span></span>

<span data-ttu-id="ebe28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebe28-105">Informações de data e hora para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="ebe28-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebe28-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebe28-106">JSON representation</span></span>

<span data-ttu-id="ebe28-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ebe28-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ebe28-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebe28-108">Properties</span></span>
| <span data-ttu-id="ebe28-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebe28-109">Property</span></span>     | <span data-ttu-id="ebe28-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebe28-110">Type</span></span>   |<span data-ttu-id="ebe28-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebe28-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebe28-112">data</span><span class="sxs-lookup"><span data-stu-id="ebe28-112">date</span></span>|<span data-ttu-id="ebe28-113">Data</span><span class="sxs-lookup"><span data-stu-id="ebe28-113">Date</span></span>|<span data-ttu-id="ebe28-114">A parte de data do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="ebe28-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="ebe28-115">time</span><span class="sxs-lookup"><span data-stu-id="ebe28-115">time</span></span>|<span data-ttu-id="ebe28-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ebe28-116">TimeOfDay</span></span>|<span data-ttu-id="ebe28-117">A parte de tempo do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="ebe28-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="ebe28-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="ebe28-118">timeZone</span></span>|<span data-ttu-id="ebe28-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebe28-119">String</span></span>|<span data-ttu-id="ebe28-120">A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.</span><span class="sxs-lookup"><span data-stu-id="ebe28-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
