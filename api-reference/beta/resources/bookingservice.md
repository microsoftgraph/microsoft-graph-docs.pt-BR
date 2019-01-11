---
title: tipo de recurso de bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 63eae84249501426c43ad73326cbf005009753be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815439"
---
# <a name="bookingservice-resource-type"></a><span data-ttu-id="116e3-104">tipo de recurso de bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-104">bookingService resource type</span></span>

 > <span data-ttu-id="116e3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="116e3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="116e3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="116e3-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="116e3-107">Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, preço e a equipe que geralmente fornece tal serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-107">Represents information about a particular service provided by a [bookingBusiness](bookingbusiness.md), such as the service name, price, and the staff that usually provides such service.</span></span>

## <a name="methods"></a><span data-ttu-id="116e3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="116e3-108">Methods</span></span>

| <span data-ttu-id="116e3-109">Método</span><span class="sxs-lookup"><span data-stu-id="116e3-109">Method</span></span>           | <span data-ttu-id="116e3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="116e3-110">Return Type</span></span>    |<span data-ttu-id="116e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="116e3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="116e3-112">Lista de serviços</span><span class="sxs-lookup"><span data-stu-id="116e3-112">List services</span></span>](../api/bookingbusiness-list-services.md) | <span data-ttu-id="116e3-113">coleção [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="116e3-113">[bookingService](bookingservice.md) collection</span></span> | <span data-ttu-id="116e3-114">Obtenha uma lista de objetos **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-114">Get a list of **bookingService** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="116e3-115">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-115">Create bookingService</span></span>](../api/bookingbusiness-post-services.md) | [<span data-ttu-id="116e3-116">bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-116">bookingService</span></span>](bookingservice.md) | <span data-ttu-id="116e3-117">Crie um **bookingService** para o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-117">Create a **bookingService** for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="116e3-118">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-118">Get bookingService</span></span>](../api/bookingservice-get.md) | [<span data-ttu-id="116e3-119">bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-119">bookingService</span></span>](bookingservice.md) |<span data-ttu-id="116e3-120">Obtenha as propriedades e relacionamentos de um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-120">Get the properties and relationships of a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="116e3-121">Update</span><span class="sxs-lookup"><span data-stu-id="116e3-121">Update</span></span>](../api/bookingservice-update.md) | [<span data-ttu-id="116e3-122">bookingService</span><span class="sxs-lookup"><span data-stu-id="116e3-122">bookingService</span></span>](bookingservice.md)    |<span data-ttu-id="116e3-123">Atualize um objeto **bookingService** o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-123">Update a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="116e3-124">Delete</span><span class="sxs-lookup"><span data-stu-id="116e3-124">Delete</span></span>](../api/bookingservice-delete.md) | <span data-ttu-id="116e3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="116e3-125">None</span></span> |<span data-ttu-id="116e3-126">Exclua um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="116e3-126">Delete a **bookingService** object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="116e3-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="116e3-127">Properties</span></span>
| <span data-ttu-id="116e3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="116e3-128">Property</span></span>     | <span data-ttu-id="116e3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="116e3-129">Type</span></span>   |<span data-ttu-id="116e3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="116e3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="116e3-131">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="116e3-131">defaultDuration</span></span>|<span data-ttu-id="116e3-132">Duração</span><span class="sxs-lookup"><span data-stu-id="116e3-132">Duration</span></span>|<span data-ttu-id="116e3-133">O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="116e3-133">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="116e3-134">Por exemplo, P11D23H59M59.999999999999S.</span><span class="sxs-lookup"><span data-stu-id="116e3-134">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="116e3-135">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="116e3-135">defaultLocation</span></span>|[<span data-ttu-id="116e3-136">location</span><span class="sxs-lookup"><span data-stu-id="116e3-136">location</span></span>](location.md)|<span data-ttu-id="116e3-137">A localização física padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-137">The default physical location for the service.</span></span>|
|<span data-ttu-id="116e3-138">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="116e3-138">defaultPrice</span></span>|<span data-ttu-id="116e3-139">Duplo</span><span class="sxs-lookup"><span data-stu-id="116e3-139">Double</span></span>|<span data-ttu-id="116e3-140">O preço monetários padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-140">The default monetary price for the service.</span></span>|
|<span data-ttu-id="116e3-141">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="116e3-141">defaultPriceType</span></span>|<span data-ttu-id="116e3-142">string</span><span class="sxs-lookup"><span data-stu-id="116e3-142">string</span></span>|<span data-ttu-id="116e3-143">A maneira padrão de serviço é cobrada.</span><span class="sxs-lookup"><span data-stu-id="116e3-143">The default way the service is charged.</span></span> <span data-ttu-id="116e3-144">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="116e3-144">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="116e3-145">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="116e3-145">defaultReminders</span></span>|<span data-ttu-id="116e3-146">coleção [bookingReminder](bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="116e3-146">[bookingReminder](bookingreminder.md) collection</span></span>|<span data-ttu-id="116e3-147">O padrão é definido de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-147">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="116e3-148">O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.</span><span class="sxs-lookup"><span data-stu-id="116e3-148">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="116e3-149">description</span><span class="sxs-lookup"><span data-stu-id="116e3-149">description</span></span>|<span data-ttu-id="116e3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-150">String</span></span>|<span data-ttu-id="116e3-151">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-151">A text description for the service.</span></span>|
|<span data-ttu-id="116e3-152">displayName</span><span class="sxs-lookup"><span data-stu-id="116e3-152">displayName</span></span>|<span data-ttu-id="116e3-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-153">String</span></span>|<span data-ttu-id="116e3-154">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-154">A service name.</span></span>|
|<span data-ttu-id="116e3-155">emailAddress</span><span class="sxs-lookup"><span data-stu-id="116e3-155">emailAddress</span></span>|<span data-ttu-id="116e3-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-156">String</span></span>|<span data-ttu-id="116e3-157">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="116e3-157">An email address</span></span>|
|<span data-ttu-id="116e3-158">id</span><span class="sxs-lookup"><span data-stu-id="116e3-158">id</span></span>|<span data-ttu-id="116e3-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-159">String</span></span>|<span data-ttu-id="116e3-160">A identificação desse serviço, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="116e3-160">The ID of that service, in a GUID format.</span></span> <span data-ttu-id="116e3-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="116e3-161">Read-only.</span></span>|
|<span data-ttu-id="116e3-162">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="116e3-162">isHiddenFromCustomers</span></span>|<span data-ttu-id="116e3-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="116e3-163">Boolean</span></span>|<span data-ttu-id="116e3-164">True significa que esse serviço não está disponível para os clientes de reserva.</span><span class="sxs-lookup"><span data-stu-id="116e3-164">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="116e3-165">Observações</span><span class="sxs-lookup"><span data-stu-id="116e3-165">notes</span></span>|<span data-ttu-id="116e3-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="116e3-166">String</span></span>|<span data-ttu-id="116e3-167">Informações adicionais sobre esse serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-167">Additional information about this service.</span></span>|
|<span data-ttu-id="116e3-168">postBuffer</span><span class="sxs-lookup"><span data-stu-id="116e3-168">postBuffer</span></span>|<span data-ttu-id="116e3-169">Duração</span><span class="sxs-lookup"><span data-stu-id="116e3-169">Duration</span></span>|<span data-ttu-id="116e3-170">Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.</span><span class="sxs-lookup"><span data-stu-id="116e3-170">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="116e3-171">preBuffer</span><span class="sxs-lookup"><span data-stu-id="116e3-171">preBuffer</span></span>|<span data-ttu-id="116e3-172">Duração</span><span class="sxs-lookup"><span data-stu-id="116e3-172">Duration</span></span>|<span data-ttu-id="116e3-173">O tempo de buffer antes de um compromisso para esse serviço pode iniciar.</span><span class="sxs-lookup"><span data-stu-id="116e3-173">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="116e3-174">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="116e3-174">schedulingPolicy</span></span>|[<span data-ttu-id="116e3-175">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="116e3-175">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md)|<span data-ttu-id="116e3-176">O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="116e3-176">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="116e3-177">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="116e3-177">staffMemberIds</span></span>|<span data-ttu-id="116e3-178">String collection</span><span class="sxs-lookup"><span data-stu-id="116e3-178">String collection</span></span>|<span data-ttu-id="116e3-179">Representa os [membros da equipe](bookingstaffmember.md) que forneça esse serviço.</span><span class="sxs-lookup"><span data-stu-id="116e3-179">Represents those [staff members](bookingstaffmember.md) who provide this service.</span></span> |

## <a name="relationships"></a><span data-ttu-id="116e3-180">Relações</span><span class="sxs-lookup"><span data-stu-id="116e3-180">Relationships</span></span>
<span data-ttu-id="116e3-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="116e3-181">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="116e3-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="116e3-182">JSON representation</span></span>

<span data-ttu-id="116e3-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="116e3-183">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
