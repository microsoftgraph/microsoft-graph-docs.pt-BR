---
title: tipo de recurso bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 53c5bc6be0953c68dc431be04b17f582715582c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448364"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="1ede6-104">tipo de recurso bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-104">bookingService resource type</span></span>

<span data-ttu-id="1ede6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ede6-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1ede6-106">Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-106">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="1ede6-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ede6-107">Methods</span></span>

| <span data-ttu-id="1ede6-108">Método</span><span class="sxs-lookup"><span data-stu-id="1ede6-108">Method</span></span>           | <span data-ttu-id="1ede6-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ede6-109">Return Type</span></span>    |<span data-ttu-id="1ede6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ede6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ede6-111">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="1ede6-111">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="1ede6-112">coleção [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="1ede6-112">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="1ede6-113">Obtenha uma lista de objetos **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-113">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="1ede6-114">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-114">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="1ede6-115">bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-115">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="1ede6-116">Crie um **bookingService** para o [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-116">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="1ede6-117">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-117">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="1ede6-118">bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-118">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="1ede6-119">Obtenha as propriedades e os relacionamentos de um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-119">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="1ede6-120">Update</span><span class="sxs-lookup"><span data-stu-id="1ede6-120">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="1ede6-121">bookingService</span><span class="sxs-lookup"><span data-stu-id="1ede6-121">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="1ede6-122">Atualize um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-122">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="1ede6-123">Delete</span><span class="sxs-lookup"><span data-stu-id="1ede6-123">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="1ede6-124">None</span><span class="sxs-lookup"><span data-stu-id="1ede6-124">None</span></span> |<span data-ttu-id="1ede6-125">Exclua um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-125">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="1ede6-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ede6-126">Properties</span></span>
| <span data-ttu-id="1ede6-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ede6-127">Property</span></span>     | <span data-ttu-id="1ede6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ede6-128">Type</span></span>   |<span data-ttu-id="1ede6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ede6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ede6-130">defaultduration</span><span class="sxs-lookup"><span data-stu-id="1ede6-130">defaultDuration</span></span>|<span data-ttu-id="1ede6-131">Duração</span><span class="sxs-lookup"><span data-stu-id="1ede6-131">Duration</span></span>|<span data-ttu-id="1ede6-132">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="1ede6-132">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="1ede6-133">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="1ede6-133">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="1ede6-134">DefaultLocation</span><span class="sxs-lookup"><span data-stu-id="1ede6-134">defaultLocation</span></span>|[<span data-ttu-id="1ede6-135">location</span><span class="sxs-lookup"><span data-stu-id="1ede6-135">location</span></span>](location.md)|<span data-ttu-id="1ede6-136">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-136">The default physical location for the service.</span></span>|
|<span data-ttu-id="1ede6-137">defaultprice</span><span class="sxs-lookup"><span data-stu-id="1ede6-137">defaultPrice</span></span>|<span data-ttu-id="1ede6-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="1ede6-138">Double</span></span>|<span data-ttu-id="1ede6-139">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-139">The default monetary price for the service.</span></span>|
|<span data-ttu-id="1ede6-140">defaultpricetype</span><span class="sxs-lookup"><span data-stu-id="1ede6-140">defaultPriceType</span></span>|<span data-ttu-id="1ede6-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ede6-141">string</span></span>|<span data-ttu-id="1ede6-142">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-142">The default way the service is charged.</span></span> <span data-ttu-id="1ede6-143">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="1ede6-143">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="1ede6-144">defaultlembrers</span><span class="sxs-lookup"><span data-stu-id="1ede6-144">defaultReminders</span></span>|<span data-ttu-id="1ede6-145">coleção [bookingReminder](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="1ede6-145">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="1ede6-146">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-146">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="1ede6-147">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="1ede6-147">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="1ede6-148">description</span><span class="sxs-lookup"><span data-stu-id="1ede6-148">description</span></span>|<span data-ttu-id="1ede6-149">String</span><span class="sxs-lookup"><span data-stu-id="1ede6-149">String</span></span>|<span data-ttu-id="1ede6-150">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-150">A text description for the service.</span></span>|
|<span data-ttu-id="1ede6-151">displayName</span><span class="sxs-lookup"><span data-stu-id="1ede6-151">displayName</span></span>|<span data-ttu-id="1ede6-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ede6-152">String</span></span>|<span data-ttu-id="1ede6-153">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-153">A service name.</span></span>|
|<span data-ttu-id="1ede6-154">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1ede6-154">emailAddress</span></span>|<span data-ttu-id="1ede6-155">String</span><span class="sxs-lookup"><span data-stu-id="1ede6-155">String</span></span>|<span data-ttu-id="1ede6-156">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="1ede6-156">An email address</span></span>|
|<span data-ttu-id="1ede6-157">id</span><span class="sxs-lookup"><span data-stu-id="1ede6-157">id</span></span>|<span data-ttu-id="1ede6-158">String</span><span class="sxs-lookup"><span data-stu-id="1ede6-158">String</span></span>|<span data-ttu-id="1ede6-159">A ID do serviço, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1ede6-159">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="1ede6-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ede6-160">Read-only.</span></span>|
|<span data-ttu-id="1ede6-161">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="1ede6-161">isHiddenFromCustomers</span></span>|<span data-ttu-id="1ede6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ede6-162">Boolean</span></span>|<span data-ttu-id="1ede6-163">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="1ede6-163">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="1ede6-164">notes</span><span class="sxs-lookup"><span data-stu-id="1ede6-164">notes</span></span>|<span data-ttu-id="1ede6-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ede6-165">String</span></span>|<span data-ttu-id="1ede6-166">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-166">Additional information about this service.</span></span>|
|<span data-ttu-id="1ede6-167">Buffer</span><span class="sxs-lookup"><span data-stu-id="1ede6-167">postBuffer</span></span>|<span data-ttu-id="1ede6-168">Duração</span><span class="sxs-lookup"><span data-stu-id="1ede6-168">Duration</span></span>|<span data-ttu-id="1ede6-169">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-169">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="1ede6-170">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="1ede6-170">preBuffer</span></span>|<span data-ttu-id="1ede6-171">Duração</span><span class="sxs-lookup"><span data-stu-id="1ede6-171">Duration</span></span>|<span data-ttu-id="1ede6-172">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="1ede6-172">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="1ede6-173">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="1ede6-173">schedulingPolicy</span></span>|[<span data-ttu-id="1ede6-174">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="1ede6-174">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="1ede6-175">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1ede6-175">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="1ede6-176">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="1ede6-176">staffMemberIds</span></span>|<span data-ttu-id="1ede6-177">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1ede6-177">String collection</span></span>|<span data-ttu-id="1ede6-178">Representa os [membros da equipe](bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="1ede6-178">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1ede6-179">Relações</span><span class="sxs-lookup"><span data-stu-id="1ede6-179">Relationships</span></span>
<span data-ttu-id="1ede6-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ede6-180">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1ede6-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ede6-181">JSON representation</span></span>

<span data-ttu-id="1ede6-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ede6-182">The following is a JSON representation of the resource.</span></span>

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
