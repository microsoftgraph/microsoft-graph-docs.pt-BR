---
title: tipo de recurso attendanceInterval
description: Contém informações associadas ao intervalo de participação no attendanceRecord.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896512"
---
# <a name="attendanceinterval-resource-type"></a><span data-ttu-id="33fd4-103">tipo de recurso attendanceInterval</span><span class="sxs-lookup"><span data-stu-id="33fd4-103">attendanceInterval resource type</span></span>

<span data-ttu-id="33fd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33fd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33fd4-105">Contém informações associadas ao intervalo de participação no attendanceRecord.</span><span class="sxs-lookup"><span data-stu-id="33fd4-105">Contains information associated with attendance interval in attendanceRecord.</span></span>

## <a name="properties"></a><span data-ttu-id="33fd4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33fd4-106">Properties</span></span>

| <span data-ttu-id="33fd4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33fd4-107">Property</span></span>            | <span data-ttu-id="33fd4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="33fd4-108">Type</span></span>    | <span data-ttu-id="33fd4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33fd4-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="33fd4-110">joinDateTime</span><span class="sxs-lookup"><span data-stu-id="33fd4-110">joinDateTime</span></span> | <span data-ttu-id="33fd4-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="33fd4-111">DateTime</span></span> | <span data-ttu-id="33fd4-112">Participante do horário ingressado em UTC.</span><span class="sxs-lookup"><span data-stu-id="33fd4-112">Time attendee joined in UTC.</span></span> |
| <span data-ttu-id="33fd4-113">leaveDateTime</span><span class="sxs-lookup"><span data-stu-id="33fd4-113">leaveDateTime</span></span> | <span data-ttu-id="33fd4-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="33fd4-114">DateTime</span></span> | <span data-ttu-id="33fd4-115">O participante do horário foi deixado em UTC.</span><span class="sxs-lookup"><span data-stu-id="33fd4-115">Time attendee left in UTC.</span></span> |
| <span data-ttu-id="33fd4-116">durationInSeconds</span><span class="sxs-lookup"><span data-stu-id="33fd4-116">durationInSeconds</span></span> | <span data-ttu-id="33fd4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="33fd4-117">Int32</span></span> | <span data-ttu-id="33fd4-118">Duração do intervalo de reunião em segundos; ou seja, a diferença entre **joinDateTime** e **leaveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="33fd4-118">Duration of the meeting interval in seconds; that is, the difference between **joinDateTime** and **leaveDateTime**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33fd4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33fd4-119">JSON representation</span></span>

<span data-ttu-id="33fd4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33fd4-120">The following is a JSON representation of the resource.</span></span>

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
