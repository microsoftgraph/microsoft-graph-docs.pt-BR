---
title: tipo de recurso bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 685f4136b5b16c09d8fa53c385d75312a9337870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507912"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="201af-104">tipo de recurso bookingReminder</span><span class="sxs-lookup"><span data-stu-id="201af-104">bookingReminder resource type</span></span>

<span data-ttu-id="201af-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="201af-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="201af-106">Representa quando e para quem enviar um lembrete de email.</span><span class="sxs-lookup"><span data-stu-id="201af-106">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="201af-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="201af-107">Properties</span></span>
| <span data-ttu-id="201af-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="201af-108">Property</span></span>     | <span data-ttu-id="201af-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="201af-109">Type</span></span>   |<span data-ttu-id="201af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="201af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="201af-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="201af-111">message</span></span>|<span data-ttu-id="201af-112">String</span><span class="sxs-lookup"><span data-stu-id="201af-112">String</span></span>|<span data-ttu-id="201af-113">A mensagem no lembrete.</span><span class="sxs-lookup"><span data-stu-id="201af-113">The message in the reminder.</span></span>|
|<span data-ttu-id="201af-114">partida</span><span class="sxs-lookup"><span data-stu-id="201af-114">offset</span></span>|<span data-ttu-id="201af-115">Duração</span><span class="sxs-lookup"><span data-stu-id="201af-115">Duration</span></span>|<span data-ttu-id="201af-116">O período de tempo antes do início de um compromisso para o qual o lembrete deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="201af-116">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="201af-117">Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="201af-117">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="201af-118">destinatários</span><span class="sxs-lookup"><span data-stu-id="201af-118">recipients</span></span>|<span data-ttu-id="201af-119">String</span><span class="sxs-lookup"><span data-stu-id="201af-119">String</span></span>| <span data-ttu-id="201af-120">As pessoas que shouold receberão o lembrete.</span><span class="sxs-lookup"><span data-stu-id="201af-120">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="201af-121">Os valores possíveis são: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="201af-121">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="201af-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="201af-122">JSON representation</span></span>

<span data-ttu-id="201af-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="201af-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
