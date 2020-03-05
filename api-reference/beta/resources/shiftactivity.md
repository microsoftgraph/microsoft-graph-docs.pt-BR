---
title: tipo de recurso shiftActivity
description: Representa uma atividade em um turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6adc82eca2c7ce53713997c18001aef19c76e3dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520629"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="b0c11-103">tipo de recurso shiftActivity</span><span class="sxs-lookup"><span data-stu-id="b0c11-103">shiftActivity resource type</span></span>

<span data-ttu-id="b0c11-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0c11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c11-105">Representa uma atividade em um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="b0c11-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b0c11-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c11-106">Properties</span></span>
| <span data-ttu-id="b0c11-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c11-107">Property</span></span>                         | <span data-ttu-id="b0c11-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c11-108">Type</span></span>                    | <span data-ttu-id="b0c11-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c11-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b0c11-110">ispago</span><span class="sxs-lookup"><span data-stu-id="b0c11-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="b0c11-111">Indica se o `microsoft.graph.user` deve ser pago para a atividade durante seu `shift`.</span><span class="sxs-lookup"><span data-stu-id="b0c11-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="b0c11-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c11-112">Required.</span></span>    |
| <span data-ttu-id="b0c11-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c11-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b0c11-114">A data e a hora de início `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="b0c11-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b0c11-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b0c11-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0c11-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b0c11-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b0c11-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c11-117">Required.</span></span> |
| <span data-ttu-id="b0c11-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c11-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b0c11-119">A data e a hora de término `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="b0c11-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b0c11-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b0c11-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0c11-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b0c11-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b0c11-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c11-122">Required.</span></span>    |
| <span data-ttu-id="b0c11-123">código</span><span class="sxs-lookup"><span data-stu-id="b0c11-123">code</span></span>               | `string`                  | <span data-ttu-id="b0c11-124">Código definido pelo cliente para `shiftActivity`o.</span><span class="sxs-lookup"><span data-stu-id="b0c11-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="b0c11-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c11-125">Required.</span></span>    |
| <span data-ttu-id="b0c11-126">displayName</span><span class="sxs-lookup"><span data-stu-id="b0c11-126">displayName</span></span>               | `string`                  | <span data-ttu-id="b0c11-127">O nome do `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="b0c11-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="b0c11-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c11-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b0c11-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c11-129">JSON representation</span></span>

<span data-ttu-id="b0c11-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c11-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
