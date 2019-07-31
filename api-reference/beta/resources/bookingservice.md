---
title: tipo de recurso bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5f51ec999f0a2048b8dbcbdd533c609eb5a86757
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974126"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="dad3f-104">tipo de recurso bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="dad3f-105">Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="dad3f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dad3f-106">Methods</span></span>

| <span data-ttu-id="dad3f-107">Método</span><span class="sxs-lookup"><span data-stu-id="dad3f-107">Method</span></span>           | <span data-ttu-id="dad3f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dad3f-108">Return Type</span></span>    |<span data-ttu-id="dad3f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad3f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dad3f-110">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="dad3f-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="dad3f-111">coleção [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="dad3f-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="dad3f-112">Obtenha uma lista de objetos **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="dad3f-113">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="dad3f-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="dad3f-115">Crie um **bookingService** para o [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="dad3f-116">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="dad3f-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="dad3f-118">Obtenha as propriedades e os relacionamentos de um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="dad3f-119">Atualização</span><span class="sxs-lookup"><span data-stu-id="dad3f-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="dad3f-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="dad3f-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="dad3f-121">Atualize um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="dad3f-122">Delete</span><span class="sxs-lookup"><span data-stu-id="dad3f-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="dad3f-123">None</span><span class="sxs-lookup"><span data-stu-id="dad3f-123">None</span></span> |<span data-ttu-id="dad3f-124">Exclua um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="dad3f-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dad3f-125">Properties</span></span>
| <span data-ttu-id="dad3f-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dad3f-126">Property</span></span>     | <span data-ttu-id="dad3f-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="dad3f-127">Type</span></span>   |<span data-ttu-id="dad3f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad3f-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad3f-129">defaultduration</span><span class="sxs-lookup"><span data-stu-id="dad3f-129">defaultDuration</span></span>|<span data-ttu-id="dad3f-130">Duração</span><span class="sxs-lookup"><span data-stu-id="dad3f-130">Duration</span></span>|<span data-ttu-id="dad3f-131">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="dad3f-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="dad3f-132">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="dad3f-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="dad3f-133">DefaultLocation</span><span class="sxs-lookup"><span data-stu-id="dad3f-133">defaultLocation</span></span>|[<span data-ttu-id="dad3f-134">location</span><span class="sxs-lookup"><span data-stu-id="dad3f-134">location</span></span>](location.md)|<span data-ttu-id="dad3f-135">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="dad3f-136">defaultprice</span><span class="sxs-lookup"><span data-stu-id="dad3f-136">defaultPrice</span></span>|<span data-ttu-id="dad3f-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="dad3f-137">Double</span></span>|<span data-ttu-id="dad3f-138">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="dad3f-139">defaultpricetype</span><span class="sxs-lookup"><span data-stu-id="dad3f-139">defaultPriceType</span></span>|<span data-ttu-id="dad3f-140">string</span><span class="sxs-lookup"><span data-stu-id="dad3f-140">string</span></span>|<span data-ttu-id="dad3f-141">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-141">The default way the service is charged.</span></span> <span data-ttu-id="dad3f-142">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="dad3f-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="dad3f-143">defaultlembrers</span><span class="sxs-lookup"><span data-stu-id="dad3f-143">defaultReminders</span></span>|<span data-ttu-id="dad3f-144">coleção [bookingReminder](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="dad3f-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="dad3f-145">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="dad3f-146">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="dad3f-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="dad3f-147">descrição</span><span class="sxs-lookup"><span data-stu-id="dad3f-147">description</span></span>|<span data-ttu-id="dad3f-148">String</span><span class="sxs-lookup"><span data-stu-id="dad3f-148">String</span></span>|<span data-ttu-id="dad3f-149">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-149">A text description for the service.</span></span>|
|<span data-ttu-id="dad3f-150">displayName</span><span class="sxs-lookup"><span data-stu-id="dad3f-150">displayName</span></span>|<span data-ttu-id="dad3f-151">String</span><span class="sxs-lookup"><span data-stu-id="dad3f-151">String</span></span>|<span data-ttu-id="dad3f-152">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-152">A service name.</span></span>|
|<span data-ttu-id="dad3f-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dad3f-153">emailAddress</span></span>|<span data-ttu-id="dad3f-154">String</span><span class="sxs-lookup"><span data-stu-id="dad3f-154">String</span></span>|<span data-ttu-id="dad3f-155">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="dad3f-155">An email address</span></span>|
|<span data-ttu-id="dad3f-156">id</span><span class="sxs-lookup"><span data-stu-id="dad3f-156">id</span></span>|<span data-ttu-id="dad3f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad3f-157">String</span></span>|<span data-ttu-id="dad3f-158">A ID do serviço, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="dad3f-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="dad3f-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dad3f-159">Read-only.</span></span>|
|<span data-ttu-id="dad3f-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="dad3f-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="dad3f-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="dad3f-161">Boolean</span></span>|<span data-ttu-id="dad3f-162">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="dad3f-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="dad3f-163">notes</span><span class="sxs-lookup"><span data-stu-id="dad3f-163">notes</span></span>|<span data-ttu-id="dad3f-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad3f-164">String</span></span>|<span data-ttu-id="dad3f-165">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-165">Additional information about this service.</span></span>|
|<span data-ttu-id="dad3f-166">Buffer</span><span class="sxs-lookup"><span data-stu-id="dad3f-166">postBuffer</span></span>|<span data-ttu-id="dad3f-167">Duração</span><span class="sxs-lookup"><span data-stu-id="dad3f-167">Duration</span></span>|<span data-ttu-id="dad3f-168">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="dad3f-169">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="dad3f-169">preBuffer</span></span>|<span data-ttu-id="dad3f-170">Duração</span><span class="sxs-lookup"><span data-stu-id="dad3f-170">Duration</span></span>|<span data-ttu-id="dad3f-171">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="dad3f-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="dad3f-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="dad3f-172">schedulingPolicy</span></span>|[<span data-ttu-id="dad3f-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="dad3f-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="dad3f-174">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="dad3f-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="dad3f-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="dad3f-175">staffMemberIds</span></span>|<span data-ttu-id="dad3f-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dad3f-176">String collection</span></span>|<span data-ttu-id="dad3f-177">Representa os [membros da equipe](bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="dad3f-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dad3f-178">Relações</span><span class="sxs-lookup"><span data-stu-id="dad3f-178">Relationships</span></span>
<span data-ttu-id="dad3f-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dad3f-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dad3f-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dad3f-180">JSON representation</span></span>

<span data-ttu-id="dad3f-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dad3f-181">The following is a JSON representation of the resource.</span></span>

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
