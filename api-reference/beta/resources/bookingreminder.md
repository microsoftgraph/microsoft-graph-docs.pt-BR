---
title: tipo de recurso bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a87f504824136fc1f3e3639361e22f78c6719dba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974133"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="44225-104">tipo de recurso bookingReminder</span><span class="sxs-lookup"><span data-stu-id="44225-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="44225-105">Representa quando e para quem enviar um lembrete de email.</span><span class="sxs-lookup"><span data-stu-id="44225-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="44225-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44225-106">Properties</span></span>
| <span data-ttu-id="44225-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44225-107">Property</span></span>     | <span data-ttu-id="44225-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44225-108">Type</span></span>   |<span data-ttu-id="44225-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44225-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44225-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="44225-110">message</span></span>|<span data-ttu-id="44225-111">String</span><span class="sxs-lookup"><span data-stu-id="44225-111">String</span></span>|<span data-ttu-id="44225-112">A mensagem no lembrete.</span><span class="sxs-lookup"><span data-stu-id="44225-112">The message in the reminder.</span></span>|
|<span data-ttu-id="44225-113">partida</span><span class="sxs-lookup"><span data-stu-id="44225-113">offset</span></span>|<span data-ttu-id="44225-114">Duração</span><span class="sxs-lookup"><span data-stu-id="44225-114">Duration</span></span>|<span data-ttu-id="44225-115">O período de tempo antes do início de um compromisso para o qual o lembrete deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="44225-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="44225-116">Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="44225-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="44225-117">destinatários</span><span class="sxs-lookup"><span data-stu-id="44225-117">recipients</span></span>|<span data-ttu-id="44225-118">String</span><span class="sxs-lookup"><span data-stu-id="44225-118">String</span></span>| <span data-ttu-id="44225-119">As pessoas que shouold receberão o lembrete.</span><span class="sxs-lookup"><span data-stu-id="44225-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="44225-120">Os valores possíveis são: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="44225-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44225-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44225-121">JSON representation</span></span>

<span data-ttu-id="44225-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44225-122">The following is a JSON representation of the resource.</span></span>

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
