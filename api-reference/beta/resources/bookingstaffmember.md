---
title: tipo de recurso bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543724"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="232ff-104">tipo de recurso bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="232ff-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="232ff-105">Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="232ff-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="232ff-106">Os membros da equipe podem fazer parte do locatário do Office 355 onde o negócio de reserva está configurado ou podem usar os serviços de email de outros provedores de email.</span><span class="sxs-lookup"><span data-stu-id="232ff-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="232ff-107">Ao reservar compromissos, a API Books considera as seguintes configurações para determinar a disponibilidade de um membro da equipe:</span><span class="sxs-lookup"><span data-stu-id="232ff-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="232ff-108">Por padrão, as horas de operação da empresa (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representam a disponibilidade geral do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="232ff-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="232ff-109">Se **useBusinessHours** for false, o horário de trabalho específico do membro da equipe (propriedade**WorkingHours** da entidade **bookingStaffmember** ) representará a disponibilidade geral do membro.</span><span class="sxs-lookup"><span data-stu-id="232ff-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="232ff-110">Se **availabilityIsAffectedByPersonalCalendar** for true, a API Books primeiro examinaria as horas do membro da equipe em geral (conforme determinado por #1 ou #2) e verificará a disponibilidade dessas horas no pessoal do membro da equipe calendário, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="232ff-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="232ff-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="232ff-111">Methods</span></span>

| <span data-ttu-id="232ff-112">Método</span><span class="sxs-lookup"><span data-stu-id="232ff-112">Method</span></span>           | <span data-ttu-id="232ff-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="232ff-113">Return Type</span></span>    |<span data-ttu-id="232ff-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="232ff-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="232ff-115">Listar membros da equipe</span><span class="sxs-lookup"><span data-stu-id="232ff-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="232ff-116">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="232ff-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="232ff-117">Obtenha uma lista de objetos **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="232ff-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="232ff-118">Criar bookingStaff</span><span class="sxs-lookup"><span data-stu-id="232ff-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="232ff-119">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="232ff-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="232ff-120">Criar um novo **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="232ff-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="232ff-121">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="232ff-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="232ff-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="232ff-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="232ff-123">Obtenha as propriedades e os relacionamentos de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="232ff-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="232ff-124">Update</span><span class="sxs-lookup"><span data-stu-id="232ff-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="232ff-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="232ff-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="232ff-126">Atualiza as propriedades de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="232ff-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="232ff-127">Excluir</span><span class="sxs-lookup"><span data-stu-id="232ff-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="232ff-128">None</span><span class="sxs-lookup"><span data-stu-id="232ff-128">None</span></span> |<span data-ttu-id="232ff-129">Excluir um membro da equipe no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="232ff-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="232ff-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="232ff-130">Properties</span></span>
| <span data-ttu-id="232ff-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="232ff-131">Property</span></span>     | <span data-ttu-id="232ff-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="232ff-132">Type</span></span>   |<span data-ttu-id="232ff-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="232ff-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="232ff-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="232ff-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="232ff-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="232ff-135">Boolean</span></span>|<span data-ttu-id="232ff-136">True significa que, se o membro da equipe for um usuário do Office 365, a API de reservas verificará a disponibilidade do membro da equipe em seu calendário pessoal no Office 365, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="232ff-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="232ff-137">colorIndex</span><span class="sxs-lookup"><span data-stu-id="232ff-137">colorIndex</span></span>|<span data-ttu-id="232ff-138">Int32</span><span class="sxs-lookup"><span data-stu-id="232ff-138">Int32</span></span>|<span data-ttu-id="232ff-139">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="232ff-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="232ff-140">A cor corresponde à paleta de cores na página de **detalhes da equipe** no aplicativo de reservas.</span><span class="sxs-lookup"><span data-stu-id="232ff-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="232ff-141">displayName</span><span class="sxs-lookup"><span data-stu-id="232ff-141">displayName</span></span>|<span data-ttu-id="232ff-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="232ff-142">String</span></span>|<span data-ttu-id="232ff-143">O nome do membro da equipe, conforme exibido para os clientes.</span><span class="sxs-lookup"><span data-stu-id="232ff-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="232ff-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="232ff-144">Required.</span></span>|
|<span data-ttu-id="232ff-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="232ff-145">emailAddress</span></span>|<span data-ttu-id="232ff-146">String</span><span class="sxs-lookup"><span data-stu-id="232ff-146">String</span></span>|<span data-ttu-id="232ff-147">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="232ff-147">The email address of the staff member.</span></span> <span data-ttu-id="232ff-148">Isso pode ser no mesmo locatário do Office 365 que a empresa ou em um domínio de email diferente.</span><span class="sxs-lookup"><span data-stu-id="232ff-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="232ff-149">Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa.</span><span class="sxs-lookup"><span data-stu-id="232ff-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="232ff-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="232ff-150">Required.</span></span>|
|<span data-ttu-id="232ff-151">id</span><span class="sxs-lookup"><span data-stu-id="232ff-151">id</span></span>|<span data-ttu-id="232ff-152">String</span><span class="sxs-lookup"><span data-stu-id="232ff-152">String</span></span>| <span data-ttu-id="232ff-153">A ID do membro da equipe, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="232ff-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="232ff-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="232ff-154">Read-only.</span></span>|
|<span data-ttu-id="232ff-155">role</span><span class="sxs-lookup"><span data-stu-id="232ff-155">role</span></span>|<span data-ttu-id="232ff-156">string</span><span class="sxs-lookup"><span data-stu-id="232ff-156">string</span></span>| <span data-ttu-id="232ff-157">A função do membro da equipe na empresa.</span><span class="sxs-lookup"><span data-stu-id="232ff-157">The role of the staff member in the business.</span></span> <span data-ttu-id="232ff-158">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="232ff-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="232ff-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="232ff-159">Required.</span></span>|
|<span data-ttu-id="232ff-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="232ff-160">useBusinessHours</span></span>|<span data-ttu-id="232ff-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="232ff-161">Boolean</span></span>|<span data-ttu-id="232ff-162">True significa que a disponibilidade do membro da equipe é conforme especificado na propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="232ff-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="232ff-163">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="232ff-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="232ff-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="232ff-164">workingHours</span></span>|<span data-ttu-id="232ff-165">coleção [bookingWorkHours](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="232ff-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="232ff-166">O intervalo de horas por dia da semana em que o membro da equipe está disponível para reserva.</span><span class="sxs-lookup"><span data-stu-id="232ff-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="232ff-167">Por padrão, eles são inicializados de acordo com a propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="232ff-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="232ff-168">Relações</span><span class="sxs-lookup"><span data-stu-id="232ff-168">Relationships</span></span>
<span data-ttu-id="232ff-169">Nenhum</span><span class="sxs-lookup"><span data-stu-id="232ff-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="232ff-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="232ff-170">JSON representation</span></span>

<span data-ttu-id="232ff-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="232ff-171">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
