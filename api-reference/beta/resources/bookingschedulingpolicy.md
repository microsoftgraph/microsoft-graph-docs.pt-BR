---
title: tipo de recurso bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1d3c55961161ea820eac97baa0da2ad2daf24cd2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328254"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="cd946-104">tipo de recurso bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="cd946-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="cd946-105">Representa o conjunto de políticas que determinam como os compromissos devem ser criados em um calendário do Microsoft bookings.</span><span class="sxs-lookup"><span data-stu-id="cd946-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="cd946-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd946-106">Properties</span></span>
| <span data-ttu-id="cd946-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd946-107">Property</span></span>     | <span data-ttu-id="cd946-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd946-108">Type</span></span>   |<span data-ttu-id="cd946-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd946-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd946-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="cd946-110">allowStaffSelection</span></span>|<span data-ttu-id="cd946-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd946-111">Boolean</span></span>|<span data-ttu-id="cd946-112">True se para permitir que os clientes escolham uma pessoa específica para a reserva.</span><span class="sxs-lookup"><span data-stu-id="cd946-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="cd946-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="cd946-113">maximumAdvance</span></span>|<span data-ttu-id="cd946-114">Duração</span><span class="sxs-lookup"><span data-stu-id="cd946-114">Duration</span></span>|<span data-ttu-id="cd946-115">Número máximo de dias de antecedência que uma reserva pode ser feita.</span><span class="sxs-lookup"><span data-stu-id="cd946-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="cd946-116">Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="cd946-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="cd946-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="cd946-117">minimumLeadTime</span></span>|<span data-ttu-id="cd946-118">Duração</span><span class="sxs-lookup"><span data-stu-id="cd946-118">Duration</span></span>|<span data-ttu-id="cd946-119">A quantidade mínima de tempo antes da qual as reservas e os cancelamentos devem ser feitos.</span><span class="sxs-lookup"><span data-stu-id="cd946-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="cd946-120">Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="cd946-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="cd946-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="cd946-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="cd946-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd946-122">Boolean</span></span>| <span data-ttu-id="cd946-123">True para notificar a empresa por email quando uma reserva é criada ou alterada.</span><span class="sxs-lookup"><span data-stu-id="cd946-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="cd946-124">Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para a empresa.</span><span class="sxs-lookup"><span data-stu-id="cd946-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="cd946-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="cd946-125">timeSlotInterval</span></span>|<span data-ttu-id="cd946-126">Duração</span><span class="sxs-lookup"><span data-stu-id="cd946-126">Duration</span></span>|<span data-ttu-id="cd946-127">Duração de cada intervalo de tempo, indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="cd946-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd946-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd946-128">JSON representation</span></span>

<span data-ttu-id="cd946-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd946-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
