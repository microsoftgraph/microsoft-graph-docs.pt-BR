---
title: tipo de recurso bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 59884eaf1fa3227214b00936298a4adee5a7491f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448371"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="d64c4-104">tipo de recurso bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d64c4-104">bookingSchedulingPolicy resource type</span></span>

<span data-ttu-id="d64c4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d64c4-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d64c4-106">Representa o conjunto de políticas que determinam como os compromissos devem ser criados em um calendário do Microsoft bookings.</span><span class="sxs-lookup"><span data-stu-id="d64c4-106">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="d64c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d64c4-107">Properties</span></span>
| <span data-ttu-id="d64c4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d64c4-108">Property</span></span>     | <span data-ttu-id="d64c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d64c4-109">Type</span></span>   |<span data-ttu-id="d64c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d64c4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d64c4-111">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="d64c4-111">allowStaffSelection</span></span>|<span data-ttu-id="d64c4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64c4-112">Boolean</span></span>|<span data-ttu-id="d64c4-113">True se para permitir que os clientes escolham uma pessoa específica para a reserva.</span><span class="sxs-lookup"><span data-stu-id="d64c4-113">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="d64c4-114">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="d64c4-114">maximumAdvance</span></span>|<span data-ttu-id="d64c4-115">Duração</span><span class="sxs-lookup"><span data-stu-id="d64c4-115">Duration</span></span>|<span data-ttu-id="d64c4-116">Número máximo de dias de antecedência que uma reserva pode ser feita.</span><span class="sxs-lookup"><span data-stu-id="d64c4-116">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="d64c4-117">Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="d64c4-117">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="d64c4-118">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="d64c4-118">minimumLeadTime</span></span>|<span data-ttu-id="d64c4-119">Duração</span><span class="sxs-lookup"><span data-stu-id="d64c4-119">Duration</span></span>|<span data-ttu-id="d64c4-120">A quantidade mínima de tempo antes da qual as reservas e os cancelamentos devem ser feitos.</span><span class="sxs-lookup"><span data-stu-id="d64c4-120">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="d64c4-121">Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="d64c4-121">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="d64c4-122">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="d64c4-122">sendConfirmationsToOwner</span></span>|<span data-ttu-id="d64c4-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d64c4-123">Boolean</span></span>| <span data-ttu-id="d64c4-124">True para notificar a empresa por email quando uma reserva é criada ou alterada.</span><span class="sxs-lookup"><span data-stu-id="d64c4-124">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="d64c4-125">Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para a empresa.</span><span class="sxs-lookup"><span data-stu-id="d64c4-125">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="d64c4-126">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="d64c4-126">timeSlotInterval</span></span>|<span data-ttu-id="d64c4-127">Duração</span><span class="sxs-lookup"><span data-stu-id="d64c4-127">Duration</span></span>|<span data-ttu-id="d64c4-128">Duração de cada intervalo de tempo, indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="d64c4-128">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d64c4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d64c4-129">JSON representation</span></span>

<span data-ttu-id="d64c4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d64c4-130">The following is a JSON representation of the resource.</span></span>

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
