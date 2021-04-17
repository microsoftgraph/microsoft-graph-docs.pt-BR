---
title: Tipo de recurso meetingAttendanceReport
description: Contém informações associadas ao relatório de participação na reunião.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 011250c97ae660937a1bad8e008e4932bb5fb289
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882640"
---
# <a name="meetingattendancereport-resource-type"></a><span data-ttu-id="8d2f2-103">Tipo de recurso meetingAttendanceReport</span><span class="sxs-lookup"><span data-stu-id="8d2f2-103">meetingAttendanceReport resource type</span></span>

<span data-ttu-id="8d2f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d2f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d2f2-105">Contém informações associadas ao relatório de participação na reunião.</span><span class="sxs-lookup"><span data-stu-id="8d2f2-105">Contains information associated with meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="8d2f2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d2f2-106">Properties</span></span>

| <span data-ttu-id="8d2f2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d2f2-107">Property</span></span>            | <span data-ttu-id="8d2f2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d2f2-108">Type</span></span>    | <span data-ttu-id="8d2f2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d2f2-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="8d2f2-110">attendanceRecords</span><span class="sxs-lookup"><span data-stu-id="8d2f2-110">attendanceRecords</span></span>           | <span data-ttu-id="8d2f2-111">[coleção attendanceRecord](attendanceRecord.md)</span><span class="sxs-lookup"><span data-stu-id="8d2f2-111">[attendanceRecord](attendanceRecord.md) collection</span></span>  | <span data-ttu-id="8d2f2-112">A lista de registros de presença.</span><span class="sxs-lookup"><span data-stu-id="8d2f2-112">The list of attendance records.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d2f2-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d2f2-113">JSON representation</span></span>

<span data-ttu-id="8d2f2-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d2f2-114">The following is a JSON representation of the resource.</span></span>

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
