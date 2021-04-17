---
title: tipo de recurso attendanceInterval
description: Contém informações associadas ao intervalo de participação no attendanceRecord.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1746adc802534f72aa9d139c6a16d8da62dd9fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882642"
---
# <a name="attendanceinterval-resource-type"></a><span data-ttu-id="b7b27-103">tipo de recurso attendanceInterval</span><span class="sxs-lookup"><span data-stu-id="b7b27-103">attendanceInterval resource type</span></span>

<span data-ttu-id="b7b27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b27-105">Contém informações associadas ao intervalo de participação no attendanceRecord.</span><span class="sxs-lookup"><span data-stu-id="b7b27-105">Contains information associated with attendance interval in attendanceRecord.</span></span>

## <a name="properties"></a><span data-ttu-id="b7b27-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7b27-106">Properties</span></span>

| <span data-ttu-id="b7b27-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7b27-107">Property</span></span>            | <span data-ttu-id="b7b27-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b27-108">Type</span></span>    | <span data-ttu-id="b7b27-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b27-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="b7b27-110">joinDateTime</span><span class="sxs-lookup"><span data-stu-id="b7b27-110">joinDateTime</span></span> | <span data-ttu-id="b7b27-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="b7b27-111">DateTime</span></span> | <span data-ttu-id="b7b27-112">Participante do horário ingressado em UTC.</span><span class="sxs-lookup"><span data-stu-id="b7b27-112">Time attendee joined in UTC.</span></span> |
| <span data-ttu-id="b7b27-113">leaveDateTime</span><span class="sxs-lookup"><span data-stu-id="b7b27-113">leaveDateTime</span></span> | <span data-ttu-id="b7b27-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="b7b27-114">DateTime</span></span> | <span data-ttu-id="b7b27-115">O participante do horário foi deixado em UTC.</span><span class="sxs-lookup"><span data-stu-id="b7b27-115">Time attendee left in UTC.</span></span> |
| <span data-ttu-id="b7b27-116">durationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b7b27-116">durationInSeconds</span></span> | <span data-ttu-id="b7b27-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b7b27-117">Int32</span></span> | <span data-ttu-id="b7b27-118">Duração do intervalo de reunião em segundos; ou seja, a diferença entre **joinDateTime** e **leaveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b7b27-118">Duration of the meeting interval in seconds; that is, the difference between **joinDateTime** and **leaveDateTime**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b7b27-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7b27-119">JSON representation</span></span>

<span data-ttu-id="b7b27-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7b27-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
