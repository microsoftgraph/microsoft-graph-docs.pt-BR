---
title: tipo de recurso de bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519882"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="45340-104">tipo de recurso de bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-104">bookingService resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="45340-105">Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, preço e a equipe que geralmente fornece tal serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-105">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="45340-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="45340-106">Methods</span></span>

| <span data-ttu-id="45340-107">Método</span><span class="sxs-lookup"><span data-stu-id="45340-107">Method</span></span>           | <span data-ttu-id="45340-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45340-108">Return Type</span></span>    |<span data-ttu-id="45340-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="45340-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45340-110">Lista de serviços</span><span class="sxs-lookup"><span data-stu-id="45340-110">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="45340-111">coleção [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="45340-111">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="45340-112">Obtenha uma lista de objetos **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45340-112">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="45340-113">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-113">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="45340-114">bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-114">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="45340-115">Crie um **bookingService** para o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45340-115">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="45340-116">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-116">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="45340-117">bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-117">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="45340-118">Obtenha as propriedades e relacionamentos de um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45340-118">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="45340-119">Update</span><span class="sxs-lookup"><span data-stu-id="45340-119">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="45340-120">bookingService</span><span class="sxs-lookup"><span data-stu-id="45340-120">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="45340-121">Atualize um objeto **bookingService** o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45340-121">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="45340-122">Delete</span><span class="sxs-lookup"><span data-stu-id="45340-122">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="45340-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45340-123">None</span></span> |<span data-ttu-id="45340-124">Exclua um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45340-124">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="45340-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45340-125">Properties</span></span>
| <span data-ttu-id="45340-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45340-126">Property</span></span>     | <span data-ttu-id="45340-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="45340-127">Type</span></span>   |<span data-ttu-id="45340-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="45340-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45340-129">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="45340-129">defaultDuration</span></span>|<span data-ttu-id="45340-130">Duration</span><span class="sxs-lookup"><span data-stu-id="45340-130">Duration</span></span>|<span data-ttu-id="45340-131">O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="45340-131">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="45340-132">Por exemplo, P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="45340-132">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="45340-133">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="45340-133">defaultLocation</span></span>|[<span data-ttu-id="45340-134">location</span><span class="sxs-lookup"><span data-stu-id="45340-134">location</span></span>](location.md)|<span data-ttu-id="45340-135">A localização física padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-135">The default physical location for the service.</span></span>|
|<span data-ttu-id="45340-136">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="45340-136">defaultPrice</span></span>|<span data-ttu-id="45340-137">Duplo</span><span class="sxs-lookup"><span data-stu-id="45340-137">Double</span></span>|<span data-ttu-id="45340-138">O preço monetários padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-138">The default monetary price for the service.</span></span>|
|<span data-ttu-id="45340-139">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="45340-139">defaultPriceType</span></span>|<span data-ttu-id="45340-140">string</span><span class="sxs-lookup"><span data-stu-id="45340-140">string</span></span>|<span data-ttu-id="45340-141">A maneira padrão de serviço é cobrada.</span><span class="sxs-lookup"><span data-stu-id="45340-141">The default way the service is charged.</span></span> <span data-ttu-id="45340-142">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="45340-142">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="45340-143">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="45340-143">defaultReminders</span></span>|<span data-ttu-id="45340-144">coleção [bookingReminder](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="45340-144">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="45340-145">O padrão é definido de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-145">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="45340-146">O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.</span><span class="sxs-lookup"><span data-stu-id="45340-146">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="45340-147">description</span><span class="sxs-lookup"><span data-stu-id="45340-147">description</span></span>|<span data-ttu-id="45340-148">String</span><span class="sxs-lookup"><span data-stu-id="45340-148">String</span></span>|<span data-ttu-id="45340-149">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-149">A text description for the service.</span></span>|
|<span data-ttu-id="45340-150">displayName</span><span class="sxs-lookup"><span data-stu-id="45340-150">displayName</span></span>|<span data-ttu-id="45340-151">String</span><span class="sxs-lookup"><span data-stu-id="45340-151">String</span></span>|<span data-ttu-id="45340-152">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-152">A service name.</span></span>|
|<span data-ttu-id="45340-153">emailAddress</span><span class="sxs-lookup"><span data-stu-id="45340-153">emailAddress</span></span>|<span data-ttu-id="45340-154">String</span><span class="sxs-lookup"><span data-stu-id="45340-154">String</span></span>|<span data-ttu-id="45340-155">Um email:  </span><span class="sxs-lookup"><span data-stu-id="45340-155">An email address</span></span>|
|<span data-ttu-id="45340-156">id</span><span class="sxs-lookup"><span data-stu-id="45340-156">id</span></span>|<span data-ttu-id="45340-157">String</span><span class="sxs-lookup"><span data-stu-id="45340-157">String</span></span>|<span data-ttu-id="45340-158">A identificação desse serviço, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="45340-158">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="45340-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45340-159">Read-only.</span></span>|
|<span data-ttu-id="45340-160">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="45340-160">isHiddenFromCustomers</span></span>|<span data-ttu-id="45340-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="45340-161">Boolean</span></span>|<span data-ttu-id="45340-162">True significa que esse serviço não está disponível para os clientes de reserva.</span><span class="sxs-lookup"><span data-stu-id="45340-162">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="45340-163">Observações</span><span class="sxs-lookup"><span data-stu-id="45340-163">notes</span></span>|<span data-ttu-id="45340-164">String</span><span class="sxs-lookup"><span data-stu-id="45340-164">String</span></span>|<span data-ttu-id="45340-165">Informações adicionais sobre esse serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-165">Additional information about this service.</span></span>|
|<span data-ttu-id="45340-166">postBuffer</span><span class="sxs-lookup"><span data-stu-id="45340-166">postBuffer</span></span>|<span data-ttu-id="45340-167">Duration</span><span class="sxs-lookup"><span data-stu-id="45340-167">Duration</span></span>|<span data-ttu-id="45340-168">Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.</span><span class="sxs-lookup"><span data-stu-id="45340-168">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="45340-169">preBuffer</span><span class="sxs-lookup"><span data-stu-id="45340-169">preBuffer</span></span>|<span data-ttu-id="45340-170">Duration</span><span class="sxs-lookup"><span data-stu-id="45340-170">Duration</span></span>|<span data-ttu-id="45340-171">O tempo de buffer antes de um compromisso para esse serviço pode iniciar.</span><span class="sxs-lookup"><span data-stu-id="45340-171">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="45340-172">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="45340-172">schedulingPolicy</span></span>|[<span data-ttu-id="45340-173">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="45340-173">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="45340-174">O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="45340-174">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="45340-175">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="45340-175">staffMemberIds</span></span>|<span data-ttu-id="45340-176">String collection</span><span class="sxs-lookup"><span data-stu-id="45340-176">String collection</span></span>|<span data-ttu-id="45340-177">Representa os [membros da equipe](bookingstaffmember.md) que forneça esse serviço.</span><span class="sxs-lookup"><span data-stu-id="45340-177">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="45340-178">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="45340-178">Relationships</span></span>
<span data-ttu-id="45340-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45340-179">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="45340-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45340-180">JSON representation</span></span>

<span data-ttu-id="45340-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45340-181">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
