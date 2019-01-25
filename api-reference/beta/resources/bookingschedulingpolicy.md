---
title: tipo de recurso de bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523446"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="74544-104">tipo de recurso de bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="74544-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="74544-105">Representa o conjunto de diretivas que determinam como os compromissos devem ser criados em um calendário do Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="74544-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="74544-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74544-106">Properties</span></span>
| <span data-ttu-id="74544-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74544-107">Property</span></span>     | <span data-ttu-id="74544-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="74544-108">Type</span></span>   |<span data-ttu-id="74544-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74544-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74544-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="74544-110">allowStaffSelection</span></span>|<span data-ttu-id="74544-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="74544-111">Boolean</span></span>|<span data-ttu-id="74544-112">True se permitir que os clientes escolham uma pessoa específica para a reserva.</span><span class="sxs-lookup"><span data-stu-id="74544-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="74544-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="74544-113">maximumAdvance</span></span>|<span data-ttu-id="74544-114">Duration</span><span class="sxs-lookup"><span data-stu-id="74544-114">Duration</span></span>|<span data-ttu-id="74544-115">Número máximo de dias de antecedência que pode ser feita uma reserva.</span><span class="sxs-lookup"><span data-stu-id="74544-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="74544-116">Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="74544-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="74544-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="74544-117">minimumLeadTime</span></span>|<span data-ttu-id="74544-118">Duration</span><span class="sxs-lookup"><span data-stu-id="74544-118">Duration</span></span>|<span data-ttu-id="74544-119">A quantidade mínima de tempo antes dos quais devem ser feitos reservas e cancelamentos.</span><span class="sxs-lookup"><span data-stu-id="74544-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="74544-120">Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="74544-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="74544-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="74544-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="74544-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="74544-122">Boolean</span></span>| <span data-ttu-id="74544-123">True para notificar os negócios via email quando uma reserva é criada ou alterada.</span><span class="sxs-lookup"><span data-stu-id="74544-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="74544-124">Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para os negócios.</span><span class="sxs-lookup"><span data-stu-id="74544-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="74544-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="74544-125">timeSlotInterval</span></span>|<span data-ttu-id="74544-126">Duration</span><span class="sxs-lookup"><span data-stu-id="74544-126">Duration</span></span>|<span data-ttu-id="74544-127">Duração de cada intervalo de tempo, denotado em formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="74544-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74544-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74544-128">JSON representation</span></span>

<span data-ttu-id="74544-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74544-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
