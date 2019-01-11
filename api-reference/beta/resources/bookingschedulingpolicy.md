---
title: tipo de recurso de bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 15f9e0dea22a7cfb5eab437bcc023fe3387bb2ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805359"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="b8743-104">tipo de recurso de bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b8743-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="b8743-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8743-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8743-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8743-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b8743-107">Representa o conjunto de diretivas que determinam como os compromissos devem ser criados em um calendário do Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="b8743-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="b8743-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8743-108">Properties</span></span>
| <span data-ttu-id="b8743-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8743-109">Property</span></span>     | <span data-ttu-id="b8743-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8743-110">Type</span></span>   |<span data-ttu-id="b8743-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8743-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8743-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="b8743-112">allowStaffSelection</span></span>|<span data-ttu-id="b8743-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8743-113">Boolean</span></span>|<span data-ttu-id="b8743-114">True se permitir que os clientes escolham uma pessoa específica para a reserva.</span><span class="sxs-lookup"><span data-stu-id="b8743-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="b8743-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="b8743-115">maximumAdvance</span></span>|<span data-ttu-id="b8743-116">Duração</span><span class="sxs-lookup"><span data-stu-id="b8743-116">Duration</span></span>|<span data-ttu-id="b8743-117">Número máximo de dias de antecedência que pode ser feita uma reserva.</span><span class="sxs-lookup"><span data-stu-id="b8743-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="b8743-118">Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="b8743-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="b8743-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="b8743-119">minimumLeadTime</span></span>|<span data-ttu-id="b8743-120">Duração</span><span class="sxs-lookup"><span data-stu-id="b8743-120">Duration</span></span>|<span data-ttu-id="b8743-121">A quantidade mínima de tempo antes dos quais devem ser feitos reservas e cancelamentos.</span><span class="sxs-lookup"><span data-stu-id="b8743-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="b8743-122">Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="b8743-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="b8743-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="b8743-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="b8743-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8743-124">Boolean</span></span>| <span data-ttu-id="b8743-125">True para notificar os negócios via email quando uma reserva é criada ou alterada.</span><span class="sxs-lookup"><span data-stu-id="b8743-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="b8743-126">Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para os negócios.</span><span class="sxs-lookup"><span data-stu-id="b8743-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="b8743-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="b8743-127">timeSlotInterval</span></span>|<span data-ttu-id="b8743-128">Duração</span><span class="sxs-lookup"><span data-stu-id="b8743-128">Duration</span></span>|<span data-ttu-id="b8743-129">Duração de cada intervalo de tempo, denotado em formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="b8743-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8743-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8743-130">JSON representation</span></span>

<span data-ttu-id="b8743-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8743-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
