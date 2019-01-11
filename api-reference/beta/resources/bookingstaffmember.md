---
title: tipo de recurso de bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 382da1b0710b691a6563a40c03ed62397262911d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884452"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="b8204-104">tipo de recurso de bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b8204-104">bookingStaffMember resource type</span></span>

 > <span data-ttu-id="b8204-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8204-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8204-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8204-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b8204-107">Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-107">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="b8204-108">Membros da equipe podem fazer parte do inquilino 355 Office onde os negócios de reserva está configurado, ou eles podem usar os serviços de email de outros provedores de email.</span><span class="sxs-lookup"><span data-stu-id="b8204-108">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="b8204-109">Quando os compromissos de reserva, a API de reservas considera as configurações a seguir para determinar a disponibilidade de um membro da equipe:</span><span class="sxs-lookup"><span data-stu-id="b8204-109">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="b8204-110">Por padrão, os horários de operação dos negócios (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representa a disponibilidade geral do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="b8204-110">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="b8204-111">Se **useBusinessHours** for false, horas de trabalho específico do membro da equipe (**workingHours** de propriedade da entidade **bookingStaffmember** ) representa disponibilidade geral desse membro.</span><span class="sxs-lookup"><span data-stu-id="b8204-111">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="b8204-112">Se **availabilityIsAffectedByPersonalCalendar** for true, em seguida, a API de reservas seria primeiro examine do membro da equipe geralmente disponível em horas (conforme determinado pelo #1 ou 2 #) e verifique se disponibilidade durante os horários do pessoal do membro da equipe calendário, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="b8204-112">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="b8204-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8204-113">Methods</span></span>

| <span data-ttu-id="b8204-114">Método</span><span class="sxs-lookup"><span data-stu-id="b8204-114">Method</span></span>           | <span data-ttu-id="b8204-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b8204-115">Return Type</span></span>    |<span data-ttu-id="b8204-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8204-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8204-117">Membros da equipe de lista</span><span class="sxs-lookup"><span data-stu-id="b8204-117">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="b8204-118">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="b8204-118">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b8204-119">Obtenha uma lista de objetos **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-119">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b8204-120">Criar bookingStaff</span><span class="sxs-lookup"><span data-stu-id="b8204-120">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="b8204-121">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="b8204-121">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b8204-122">Crie um novo **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-122">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b8204-123">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b8204-123">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="b8204-124">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b8204-124">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="b8204-125">Obtenha as propriedades e relacionamentos de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-125">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b8204-126">Update</span><span class="sxs-lookup"><span data-stu-id="b8204-126">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="b8204-127">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b8204-127">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="b8204-128">Atualize as propriedades de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-128">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b8204-129">Delete</span><span class="sxs-lookup"><span data-stu-id="b8204-129">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="b8204-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8204-130">None</span></span> |<span data-ttu-id="b8204-131">Exclua um membro da equipe no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b8204-131">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="b8204-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8204-132">Properties</span></span>
| <span data-ttu-id="b8204-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8204-133">Property</span></span>     | <span data-ttu-id="b8204-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8204-134">Type</span></span>   |<span data-ttu-id="b8204-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8204-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8204-136">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="b8204-136">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="b8204-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8204-137">Boolean</span></span>|<span data-ttu-id="b8204-138">True significa que se o membro da equipe é um usuário do Office 365, a API de reservas seria Verificar disponibilidade do membro da equipe no seu calendário pessoal no Office 365, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="b8204-138">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="b8204-139">colorIndex</span><span class="sxs-lookup"><span data-stu-id="b8204-139">colorIndex</span></span>|<span data-ttu-id="b8204-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b8204-140">Int32</span></span>|<span data-ttu-id="b8204-141">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="b8204-141">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="b8204-142">A cor corresponde à paleta de cores na página **detalhes da equipe** no aplicativo reservas.</span><span class="sxs-lookup"><span data-stu-id="b8204-142">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="b8204-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b8204-143">displayName</span></span>|<span data-ttu-id="b8204-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8204-144">String</span></span>|<span data-ttu-id="b8204-145">O nome do membro da equipe, como exibido aos clientes.</span><span class="sxs-lookup"><span data-stu-id="b8204-145">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="b8204-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8204-146">Required.</span></span>|
|<span data-ttu-id="b8204-147">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b8204-147">emailAddress</span></span>|<span data-ttu-id="b8204-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8204-148">String</span></span>|<span data-ttu-id="b8204-149">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="b8204-149">The email address of the staff member.</span></span> <span data-ttu-id="b8204-150">Isso pode ser em inquilino do Office 365 como a empresa ou em um domínio de email diferentes.</span><span class="sxs-lookup"><span data-stu-id="b8204-150">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="b8204-151">Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na diretiva de agendamento dos negócios.</span><span class="sxs-lookup"><span data-stu-id="b8204-151">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="b8204-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8204-152">Required.</span></span>|
|<span data-ttu-id="b8204-153">id</span><span class="sxs-lookup"><span data-stu-id="b8204-153">id</span></span>|<span data-ttu-id="b8204-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8204-154">String</span></span>| <span data-ttu-id="b8204-155">A identificação do membro da equipe, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b8204-155">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="b8204-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8204-156">Read-only.</span></span>|
|<span data-ttu-id="b8204-157">role</span><span class="sxs-lookup"><span data-stu-id="b8204-157">role</span></span>|<span data-ttu-id="b8204-158">string</span><span class="sxs-lookup"><span data-stu-id="b8204-158">string</span></span>| <span data-ttu-id="b8204-159">A função de membro da equipe de negócios.</span><span class="sxs-lookup"><span data-stu-id="b8204-159">The role of the staff member in the business.</span></span> <span data-ttu-id="b8204-160">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="b8204-160">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="b8204-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8204-161">Required.</span></span>|
|<span data-ttu-id="b8204-162">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="b8204-162">useBusinessHours</span></span>|<span data-ttu-id="b8204-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="b8204-163">Boolean</span></span>|<span data-ttu-id="b8204-164">True significa disponibilidade do membro da equipe é como especificado na propriedade **businessHours** dos negócios.</span><span class="sxs-lookup"><span data-stu-id="b8204-164">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="b8204-165">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="b8204-165">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="b8204-166">workingHours</span><span class="sxs-lookup"><span data-stu-id="b8204-166">workingHours</span></span>|<span data-ttu-id="b8204-167">coleção [bookingWorkHours](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="b8204-167">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="b8204-168">O intervalo de horas por dia da semana em que o membro da equipe está disponível para marcação.</span><span class="sxs-lookup"><span data-stu-id="b8204-168">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="b8204-169">Por padrão, eles são inicializados para ser o mesmo que a propriedade **businessHours** dos negócios.</span><span class="sxs-lookup"><span data-stu-id="b8204-169">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8204-170">Relações</span><span class="sxs-lookup"><span data-stu-id="b8204-170">Relationships</span></span>
<span data-ttu-id="b8204-171">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8204-171">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8204-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8204-172">JSON representation</span></span>

<span data-ttu-id="b8204-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8204-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
