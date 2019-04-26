---
title: tipo de recurso bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c6cf62320a6cfd8e96455e95e1d17c0621d261f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328297"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="7ce9d-104">tipo de recurso bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="7ce9d-105">Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="7ce9d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ce9d-106">Methods</span></span>

| <span data-ttu-id="7ce9d-107">Método</span><span class="sxs-lookup"><span data-stu-id="7ce9d-107">Method</span></span>           | <span data-ttu-id="7ce9d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ce9d-108">Return Type</span></span>    |<span data-ttu-id="7ce9d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce9d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ce9d-110">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="7ce9d-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="7ce9d-111">coleção [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="7ce9d-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="7ce9d-112">Obtenha uma lista de objetos **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="7ce9d-113">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="7ce9d-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="7ce9d-115">Crie um **bookingService** para o [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="7ce9d-116">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="7ce9d-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="7ce9d-118">Obtenha as propriedades e os relacionamentos de um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="7ce9d-119">Atualizar</span><span class="sxs-lookup"><span data-stu-id="7ce9d-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="7ce9d-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="7ce9d-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="7ce9d-121">Atualize um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="7ce9d-122">Delete</span><span class="sxs-lookup"><span data-stu-id="7ce9d-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="7ce9d-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7ce9d-123">None</span></span> |<span data-ttu-id="7ce9d-124">Exclua um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="7ce9d-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ce9d-125">Properties</span></span>
| <span data-ttu-id="7ce9d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ce9d-126">Property</span></span>     | <span data-ttu-id="7ce9d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ce9d-127">Type</span></span>   |<span data-ttu-id="7ce9d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ce9d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ce9d-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="7ce9d-129">defaultDuration</span></span>|<span data-ttu-id="7ce9d-130">Duração</span><span class="sxs-lookup"><span data-stu-id="7ce9d-130">Duration</span></span>|<span data-ttu-id="7ce9d-131">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="7ce9d-132">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="7ce9d-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="7ce9d-133">defaultLocation</span></span>|[<span data-ttu-id="7ce9d-134">location</span><span class="sxs-lookup"><span data-stu-id="7ce9d-134">location</span></span>](location.md)|<span data-ttu-id="7ce9d-135">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="7ce9d-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="7ce9d-136">defaultPrice</span></span>|<span data-ttu-id="7ce9d-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="7ce9d-137">Double</span></span>|<span data-ttu-id="7ce9d-138">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="7ce9d-139">defaultPricetype</span><span class="sxs-lookup"><span data-stu-id="7ce9d-139">defaultPriceType</span></span>|<span data-ttu-id="7ce9d-140">string</span><span class="sxs-lookup"><span data-stu-id="7ce9d-140">string</span></span>|<span data-ttu-id="7ce9d-141">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-141">The default way the service is charged.</span></span> <span data-ttu-id="7ce9d-142">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="7ce9d-143">defaultLembrers</span><span class="sxs-lookup"><span data-stu-id="7ce9d-143">defaultReminders</span></span>|<span data-ttu-id="7ce9d-144">coleção [bookingReminder](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="7ce9d-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="7ce9d-145">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="7ce9d-146">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="7ce9d-147">description</span><span class="sxs-lookup"><span data-stu-id="7ce9d-147">description</span></span>|<span data-ttu-id="7ce9d-148">String</span><span class="sxs-lookup"><span data-stu-id="7ce9d-148">String</span></span>|<span data-ttu-id="7ce9d-149">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-149">A text description for the service.</span></span>|
|<span data-ttu-id="7ce9d-150">displayName</span><span class="sxs-lookup"><span data-stu-id="7ce9d-150">displayName</span></span>|<span data-ttu-id="7ce9d-151">String</span><span class="sxs-lookup"><span data-stu-id="7ce9d-151">String</span></span>|<span data-ttu-id="7ce9d-152">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-152">A service name.</span></span>|
|<span data-ttu-id="7ce9d-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7ce9d-153">emailAddress</span></span>|<span data-ttu-id="7ce9d-154">String</span><span class="sxs-lookup"><span data-stu-id="7ce9d-154">String</span></span>|<span data-ttu-id="7ce9d-155">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="7ce9d-155">An email address</span></span>|
|<span data-ttu-id="7ce9d-156">id</span><span class="sxs-lookup"><span data-stu-id="7ce9d-156">id</span></span>|<span data-ttu-id="7ce9d-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ce9d-157">String</span></span>|<span data-ttu-id="7ce9d-158">A ID do serviço, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="7ce9d-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-159">Read-only.</span></span>|
|<span data-ttu-id="7ce9d-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="7ce9d-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="7ce9d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ce9d-161">Boolean</span></span>|<span data-ttu-id="7ce9d-162">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="7ce9d-163">notes</span><span class="sxs-lookup"><span data-stu-id="7ce9d-163">notes</span></span>|<span data-ttu-id="7ce9d-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ce9d-164">String</span></span>|<span data-ttu-id="7ce9d-165">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-165">Additional information about this service.</span></span>|
|<span data-ttu-id="7ce9d-166">Buffer</span><span class="sxs-lookup"><span data-stu-id="7ce9d-166">postBuffer</span></span>|<span data-ttu-id="7ce9d-167">Duração</span><span class="sxs-lookup"><span data-stu-id="7ce9d-167">Duration</span></span>|<span data-ttu-id="7ce9d-168">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="7ce9d-169">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="7ce9d-169">preBuffer</span></span>|<span data-ttu-id="7ce9d-170">Duração</span><span class="sxs-lookup"><span data-stu-id="7ce9d-170">Duration</span></span>|<span data-ttu-id="7ce9d-171">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="7ce9d-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7ce9d-172">schedulingPolicy</span></span>|[<span data-ttu-id="7ce9d-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7ce9d-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="7ce9d-174">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="7ce9d-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="7ce9d-175">staffMemberIds</span></span>|<span data-ttu-id="7ce9d-176">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7ce9d-176">String collection</span></span>|<span data-ttu-id="7ce9d-177">Representa os [membros da equipe](bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7ce9d-178">Relações</span><span class="sxs-lookup"><span data-stu-id="7ce9d-178">Relationships</span></span>
<span data-ttu-id="7ce9d-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ce9d-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7ce9d-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ce9d-180">JSON representation</span></span>

<span data-ttu-id="7ce9d-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ce9d-181">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
