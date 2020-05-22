---
title: tipo de recurso bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5ab45e1dee9c4c6fe092d07c6e1a306060e77801
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345902"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="45efc-104">tipo de recurso bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="45efc-104">bookingStaffMember resource type</span></span>

<span data-ttu-id="45efc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45efc-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="45efc-106">Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="45efc-106">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="45efc-107">Os membros da equipe podem fazer parte do locatário do Office 365 onde o negócio de reserva está configurado ou podem usar os serviços de email de outros provedores de email.</span><span class="sxs-lookup"><span data-stu-id="45efc-107">Staff members can be part of the Office 365 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="45efc-108">Ao reservar compromissos, a API Books considera as seguintes configurações para determinar a disponibilidade de um membro da equipe:</span><span class="sxs-lookup"><span data-stu-id="45efc-108">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="45efc-109">Por padrão, as horas de operação da empresa (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representam a disponibilidade geral do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="45efc-109">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="45efc-110">Se **useBusinessHours** for false, o horário de trabalho específico do membro da equipe (propriedade**WorkingHours** da entidade **bookingStaffmember** ) representará a disponibilidade geral do membro.</span><span class="sxs-lookup"><span data-stu-id="45efc-110">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="45efc-111">Se **availabilityIsAffectedByPersonalCalendar** for true, a API Books primeiro examinará as horas do membro da equipe em geral (conforme determinado pelo #1 ou #2) e verificará a disponibilidade dessas horas no calendário pessoal do membro da equipe, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="45efc-111">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="45efc-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="45efc-112">Methods</span></span>

| <span data-ttu-id="45efc-113">Método</span><span class="sxs-lookup"><span data-stu-id="45efc-113">Method</span></span>           | <span data-ttu-id="45efc-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45efc-114">Return Type</span></span>    |<span data-ttu-id="45efc-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="45efc-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="45efc-116">Listar membros da equipe</span><span class="sxs-lookup"><span data-stu-id="45efc-116">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="45efc-117">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="45efc-117">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="45efc-118">Obtenha uma lista de objetos **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="45efc-118">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="45efc-119">Criar bookingStaff</span><span class="sxs-lookup"><span data-stu-id="45efc-119">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="45efc-120">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="45efc-120">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="45efc-121">Criar um novo **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="45efc-121">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="45efc-122">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="45efc-122">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="45efc-123">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="45efc-123">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="45efc-124">Obtenha as propriedades e os relacionamentos de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="45efc-124">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="45efc-125">Atualização</span><span class="sxs-lookup"><span data-stu-id="45efc-125">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="45efc-126">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="45efc-126">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="45efc-127">Atualiza as propriedades de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="45efc-127">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="45efc-128">Delete</span><span class="sxs-lookup"><span data-stu-id="45efc-128">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="45efc-129">None</span><span class="sxs-lookup"><span data-stu-id="45efc-129">None</span></span> |<span data-ttu-id="45efc-130">Excluir um membro da equipe no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="45efc-130">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="45efc-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45efc-131">Properties</span></span>
| <span data-ttu-id="45efc-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45efc-132">Property</span></span>     | <span data-ttu-id="45efc-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="45efc-133">Type</span></span>   |<span data-ttu-id="45efc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="45efc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45efc-135">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="45efc-135">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="45efc-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="45efc-136">Boolean</span></span>|<span data-ttu-id="45efc-137">True significa que, se o membro da equipe for um usuário do Office 365, a API de reservas verificará a disponibilidade do membro da equipe em seu calendário pessoal no Office 365, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="45efc-137">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="45efc-138">colorIndex</span><span class="sxs-lookup"><span data-stu-id="45efc-138">colorIndex</span></span>|<span data-ttu-id="45efc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="45efc-139">Int32</span></span>|<span data-ttu-id="45efc-140">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="45efc-140">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="45efc-141">A cor corresponde à paleta de cores na página de **detalhes da equipe** no aplicativo de reservas.</span><span class="sxs-lookup"><span data-stu-id="45efc-141">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="45efc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="45efc-142">displayName</span></span>|<span data-ttu-id="45efc-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45efc-143">String</span></span>|<span data-ttu-id="45efc-144">O nome do membro da equipe, conforme exibido para os clientes.</span><span class="sxs-lookup"><span data-stu-id="45efc-144">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="45efc-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45efc-145">Required.</span></span>|
|<span data-ttu-id="45efc-146">emailAddress</span><span class="sxs-lookup"><span data-stu-id="45efc-146">emailAddress</span></span>|<span data-ttu-id="45efc-147">String</span><span class="sxs-lookup"><span data-stu-id="45efc-147">String</span></span>|<span data-ttu-id="45efc-148">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="45efc-148">The email address of the staff member.</span></span> <span data-ttu-id="45efc-149">Isso pode ser no mesmo locatário do Office 365 que a empresa ou em um domínio de email diferente.</span><span class="sxs-lookup"><span data-stu-id="45efc-149">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="45efc-150">Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa.</span><span class="sxs-lookup"><span data-stu-id="45efc-150">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="45efc-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45efc-151">Required.</span></span>|
|<span data-ttu-id="45efc-152">id</span><span class="sxs-lookup"><span data-stu-id="45efc-152">id</span></span>|<span data-ttu-id="45efc-153">String</span><span class="sxs-lookup"><span data-stu-id="45efc-153">String</span></span>| <span data-ttu-id="45efc-154">A ID do membro da equipe, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="45efc-154">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="45efc-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45efc-155">Read-only.</span></span>|
|<span data-ttu-id="45efc-156">role</span><span class="sxs-lookup"><span data-stu-id="45efc-156">role</span></span>|<span data-ttu-id="45efc-157">string</span><span class="sxs-lookup"><span data-stu-id="45efc-157">string</span></span>| <span data-ttu-id="45efc-158">A função do membro da equipe na empresa.</span><span class="sxs-lookup"><span data-stu-id="45efc-158">The role of the staff member in the business.</span></span> <span data-ttu-id="45efc-159">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="45efc-159">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="45efc-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45efc-160">Required.</span></span>|
|<span data-ttu-id="45efc-161">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="45efc-161">useBusinessHours</span></span>|<span data-ttu-id="45efc-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="45efc-162">Boolean</span></span>|<span data-ttu-id="45efc-163">True significa que a disponibilidade do membro da equipe é conforme especificado na propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="45efc-163">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="45efc-164">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="45efc-164">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="45efc-165">workingHours</span><span class="sxs-lookup"><span data-stu-id="45efc-165">workingHours</span></span>|<span data-ttu-id="45efc-166">coleção [bookingWorkHours](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="45efc-166">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="45efc-167">O intervalo de horas por dia da semana em que o membro da equipe está disponível para reserva.</span><span class="sxs-lookup"><span data-stu-id="45efc-167">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="45efc-168">Por padrão, eles são inicializados de acordo com a propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="45efc-168">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45efc-169">Relações</span><span class="sxs-lookup"><span data-stu-id="45efc-169">Relationships</span></span>
<span data-ttu-id="45efc-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45efc-170">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="45efc-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45efc-171">JSON representation</span></span>

<span data-ttu-id="45efc-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45efc-172">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
