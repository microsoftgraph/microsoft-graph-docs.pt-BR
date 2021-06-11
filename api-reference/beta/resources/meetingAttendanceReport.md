---
title: Tipo de recurso meetingAttendanceReport
description: Contém informações associadas ao relatório de participação na reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1ea75f6e57d0e095a470e715e080c7def05ab46
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896722"
---
# <a name="meetingattendancereport-resource-type"></a><span data-ttu-id="b0e7e-103">Tipo de recurso meetingAttendanceReport</span><span class="sxs-lookup"><span data-stu-id="b0e7e-103">meetingAttendanceReport resource type</span></span>

<span data-ttu-id="b0e7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0e7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0e7e-105">Contém informações associadas ao relatório de participação na reunião.</span><span class="sxs-lookup"><span data-stu-id="b0e7e-105">Contains information associated with meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="b0e7e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0e7e-106">Properties</span></span>

| <span data-ttu-id="b0e7e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0e7e-107">Property</span></span>            | <span data-ttu-id="b0e7e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0e7e-108">Type</span></span>    | <span data-ttu-id="b0e7e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0e7e-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="b0e7e-110">attendanceRecords</span><span class="sxs-lookup"><span data-stu-id="b0e7e-110">attendanceRecords</span></span>           | <span data-ttu-id="b0e7e-111">[coleção attendanceRecord](attendanceRecord.md)</span><span class="sxs-lookup"><span data-stu-id="b0e7e-111">[attendanceRecord](attendanceRecord.md) collection</span></span>  | <span data-ttu-id="b0e7e-112">A lista de registros de presença.</span><span class="sxs-lookup"><span data-stu-id="b0e7e-112">The list of attendance records.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0e7e-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0e7e-113">JSON representation</span></span>

<span data-ttu-id="b0e7e-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0e7e-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
