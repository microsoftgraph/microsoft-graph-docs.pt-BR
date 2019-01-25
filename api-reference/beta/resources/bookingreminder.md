---
title: tipo de recurso de bookingReminder
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526078"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="c6b62-104">tipo de recurso de bookingReminder</span><span class="sxs-lookup"><span data-stu-id="c6b62-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="c6b62-105">Representa quando e para os quais enviar um lembrete de email.</span><span class="sxs-lookup"><span data-stu-id="c6b62-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="c6b62-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6b62-106">Properties</span></span>
| <span data-ttu-id="c6b62-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6b62-107">Property</span></span>     | <span data-ttu-id="c6b62-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6b62-108">Type</span></span>   |<span data-ttu-id="c6b62-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6b62-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6b62-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="c6b62-110">message</span></span>|<span data-ttu-id="c6b62-111">String</span><span class="sxs-lookup"><span data-stu-id="c6b62-111">String</span></span>|<span data-ttu-id="c6b62-112">A mensagem do lembrete.</span><span class="sxs-lookup"><span data-stu-id="c6b62-112">The message in the reminder.</span></span>|
|<span data-ttu-id="c6b62-113">DESLOCAMENTO</span><span class="sxs-lookup"><span data-stu-id="c6b62-113">offset</span></span>|<span data-ttu-id="c6b62-114">Duration</span><span class="sxs-lookup"><span data-stu-id="c6b62-114">Duration</span></span>|<span data-ttu-id="c6b62-115">A quantidade de tempo antes do início de um compromisso que o lembrete deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="c6b62-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="c6b62-116">Ele é indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="c6b62-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="c6b62-117">recipients</span><span class="sxs-lookup"><span data-stu-id="c6b62-117">recipients</span></span>|<span data-ttu-id="c6b62-118">String</span><span class="sxs-lookup"><span data-stu-id="c6b62-118">String</span></span>| <span data-ttu-id="c6b62-119">As pessoas que recebem shouold o lembrete.</span><span class="sxs-lookup"><span data-stu-id="c6b62-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="c6b62-120">Os valores possíveis são: `allAttendees`, `staff`, `customer`.</span><span class="sxs-lookup"><span data-stu-id="c6b62-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6b62-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6b62-121">JSON representation</span></span>

<span data-ttu-id="c6b62-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6b62-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
