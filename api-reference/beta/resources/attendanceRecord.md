---
title: tipo de recurso attendanceRecord
description: Contém informações associadas ao registro de participação no relatório de participação da reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20beeca97c790b8743c9038e7fddf0b5c6f69534
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896498"
---
# <a name="attendancerecord-resource-type"></a><span data-ttu-id="97a03-103">tipo de recurso attendanceRecord</span><span class="sxs-lookup"><span data-stu-id="97a03-103">attendanceRecord resource type</span></span>

<span data-ttu-id="97a03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a03-105">Contém informações associadas ao registro de participação no relatório de participação da reunião.</span><span class="sxs-lookup"><span data-stu-id="97a03-105">Contains information associated with attendance record in meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="97a03-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97a03-106">Properties</span></span>

| <span data-ttu-id="97a03-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97a03-107">Property</span></span>            | <span data-ttu-id="97a03-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a03-108">Type</span></span>    | <span data-ttu-id="97a03-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a03-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="97a03-110">identity</span><span class="sxs-lookup"><span data-stu-id="97a03-110">identity</span></span> | [<span data-ttu-id="97a03-111">Identidade</span><span class="sxs-lookup"><span data-stu-id="97a03-111">Identity</span></span>](identity.md) | <span data-ttu-id="97a03-112">Identificador, como nome para exibição.</span><span class="sxs-lookup"><span data-stu-id="97a03-112">Identifier, such as display name.</span></span> |
| <span data-ttu-id="97a03-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="97a03-113">emailAddress</span></span> | <span data-ttu-id="97a03-114">String</span><span class="sxs-lookup"><span data-stu-id="97a03-114">String</span></span> | <span data-ttu-id="97a03-115">Endereço de email.</span><span class="sxs-lookup"><span data-stu-id="97a03-115">Email address.</span></span> |
| <span data-ttu-id="97a03-116">totalAttendanceInSeconds</span><span class="sxs-lookup"><span data-stu-id="97a03-116">totalAttendanceInSeconds</span></span> | <span data-ttu-id="97a03-117">Int32</span><span class="sxs-lookup"><span data-stu-id="97a03-117">Int32</span></span> | <span data-ttu-id="97a03-118">Duração total dos atendimentos em segundos.</span><span class="sxs-lookup"><span data-stu-id="97a03-118">Total duration of the attendances in seconds.</span></span> |
| <span data-ttu-id="97a03-119">attendanceIntervals</span><span class="sxs-lookup"><span data-stu-id="97a03-119">attendanceIntervals</span></span> | <span data-ttu-id="97a03-120">[coleção attendanceInterval](attendanceInterval.md)</span><span class="sxs-lookup"><span data-stu-id="97a03-120">[attendanceInterval](attendanceInterval.md) collection</span></span> | <span data-ttu-id="97a03-121">Lista de períodos entre a junção e a saída.</span><span class="sxs-lookup"><span data-stu-id="97a03-121">List of time periods between joining and leaving.</span></span> |
| <span data-ttu-id="97a03-122">role</span><span class="sxs-lookup"><span data-stu-id="97a03-122">role</span></span> | <span data-ttu-id="97a03-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97a03-123">String</span></span> | <span data-ttu-id="97a03-124">Função do participante.</span><span class="sxs-lookup"><span data-stu-id="97a03-124">Role of the attendee.</span></span> <span data-ttu-id="97a03-125">Os valores possíveis `None` `Attendee` são , e `Presenter` `Organizer` .</span><span class="sxs-lookup"><span data-stu-id="97a03-125">Possible values are `None`, `Attendee`, `Presenter`, and `Organizer`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="97a03-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97a03-126">JSON representation</span></span>

<span data-ttu-id="97a03-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97a03-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
