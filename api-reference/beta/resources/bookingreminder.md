---
title: tipo de recurso de bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 17cd444b8656c30e8f8966ab14571876ef9354fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936694"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="90b4a-104">tipo de recurso de bookingReminder</span><span class="sxs-lookup"><span data-stu-id="90b4a-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="90b4a-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90b4a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90b4a-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90b4a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="90b4a-107">Representa quando e para os quais enviar um lembrete de email.</span><span class="sxs-lookup"><span data-stu-id="90b4a-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="90b4a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90b4a-108">Properties</span></span>
| <span data-ttu-id="90b4a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90b4a-109">Property</span></span>     | <span data-ttu-id="90b4a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="90b4a-110">Type</span></span>   |<span data-ttu-id="90b4a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="90b4a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90b4a-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="90b4a-112">message</span></span>|<span data-ttu-id="90b4a-113">String</span><span class="sxs-lookup"><span data-stu-id="90b4a-113">String</span></span>|<span data-ttu-id="90b4a-114">A mensagem do lembrete.</span><span class="sxs-lookup"><span data-stu-id="90b4a-114">The message in the reminder.</span></span>|
|<span data-ttu-id="90b4a-115">deslocamento</span><span class="sxs-lookup"><span data-stu-id="90b4a-115">offset</span></span>|<span data-ttu-id="90b4a-116">Duração</span><span class="sxs-lookup"><span data-stu-id="90b4a-116">Duration</span></span>|<span data-ttu-id="90b4a-117">A quantidade de tempo antes do início de um compromisso que o lembrete deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="90b4a-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="90b4a-118">Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="90b4a-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="90b4a-119">recipients</span><span class="sxs-lookup"><span data-stu-id="90b4a-119">recipients</span></span>|<span data-ttu-id="90b4a-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90b4a-120">String</span></span>| <span data-ttu-id="90b4a-121">As pessoas que recebem shouold o lembrete.</span><span class="sxs-lookup"><span data-stu-id="90b4a-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="90b4a-122">Os valores possíveis são: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="90b4a-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90b4a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90b4a-123">JSON representation</span></span>

<span data-ttu-id="90b4a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90b4a-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
