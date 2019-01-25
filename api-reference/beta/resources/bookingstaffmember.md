---
title: tipo de recurso de bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520274"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="06920-104">tipo de recurso de bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06920-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="06920-105">Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="06920-106">Membros da equipe podem fazer parte do inquilino 355 Office onde os negócios de reserva está configurado, ou eles podem usar os serviços de email de outros provedores de email.</span><span class="sxs-lookup"><span data-stu-id="06920-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="06920-107">Quando os compromissos de reserva, a API de reservas considera as configurações a seguir para determinar a disponibilidade de um membro da equipe:</span><span class="sxs-lookup"><span data-stu-id="06920-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="06920-108">Por padrão, os horários de operação dos negócios (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representa a disponibilidade geral do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="06920-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="06920-109">Se **useBusinessHours** for false, horas de trabalho específico do membro da equipe (**workingHours** de propriedade da entidade **bookingStaffmember** ) representa disponibilidade geral desse membro.</span><span class="sxs-lookup"><span data-stu-id="06920-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="06920-110">Se **availabilityIsAffectedByPersonalCalendar** for true, em seguida, a API de reservas seria primeiro examine do membro da equipe geralmente disponível em horas (conforme determinado pelo #1 ou 2 #) e verifique se disponibilidade durante os horários do pessoal do membro da equipe calendário, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="06920-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="06920-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="06920-111">Methods</span></span>

| <span data-ttu-id="06920-112">Método</span><span class="sxs-lookup"><span data-stu-id="06920-112">Method</span></span>           | <span data-ttu-id="06920-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06920-113">Return Type</span></span>    |<span data-ttu-id="06920-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="06920-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06920-115">Membros da equipe de lista</span><span class="sxs-lookup"><span data-stu-id="06920-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="06920-116">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="06920-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="06920-117">Obtenha uma lista de objetos **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06920-118">Criar bookingStaff</span><span class="sxs-lookup"><span data-stu-id="06920-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="06920-119">coleção [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="06920-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="06920-120">Crie um novo **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06920-121">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06920-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="06920-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06920-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="06920-123">Obtenha as propriedades e relacionamentos de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="06920-124">Update</span><span class="sxs-lookup"><span data-stu-id="06920-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="06920-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06920-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="06920-126">Atualize as propriedades de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="06920-127">Delete</span><span class="sxs-lookup"><span data-stu-id="06920-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="06920-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06920-128">None</span></span> |<span data-ttu-id="06920-129">Exclua um membro da equipe no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="06920-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="06920-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06920-130">Properties</span></span>
| <span data-ttu-id="06920-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06920-131">Property</span></span>     | <span data-ttu-id="06920-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="06920-132">Type</span></span>   |<span data-ttu-id="06920-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="06920-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06920-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="06920-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="06920-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="06920-135">Boolean</span></span>|<span data-ttu-id="06920-136">True significa que se o membro da equipe é um usuário do Office 365, a API de reservas seria Verificar disponibilidade do membro da equipe no seu calendário pessoal no Office 365, antes de fazer uma reserva.</span><span class="sxs-lookup"><span data-stu-id="06920-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="06920-137">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="06920-137">colorIndex</span></span>|<span data-ttu-id="06920-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06920-138">Int32</span></span>|<span data-ttu-id="06920-139">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="06920-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="06920-140">A cor corresponde à paleta de cores na página **detalhes da equipe** no aplicativo reservas.</span><span class="sxs-lookup"><span data-stu-id="06920-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="06920-141">displayName</span><span class="sxs-lookup"><span data-stu-id="06920-141">displayName</span></span>|<span data-ttu-id="06920-142">String</span><span class="sxs-lookup"><span data-stu-id="06920-142">String</span></span>|<span data-ttu-id="06920-143">O nome do membro da equipe, como exibido aos clientes.</span><span class="sxs-lookup"><span data-stu-id="06920-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="06920-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06920-144">Required.</span></span>|
|<span data-ttu-id="06920-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="06920-145">emailAddress</span></span>|<span data-ttu-id="06920-146">String</span><span class="sxs-lookup"><span data-stu-id="06920-146">String</span></span>|<span data-ttu-id="06920-147">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="06920-147">The email address of the staff member.</span></span> <span data-ttu-id="06920-148">Isso pode ser em inquilino do Office 365 como a empresa ou em um domínio de email diferentes.</span><span class="sxs-lookup"><span data-stu-id="06920-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="06920-149">Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na diretiva de agendamento dos negócios.</span><span class="sxs-lookup"><span data-stu-id="06920-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="06920-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06920-150">Required.</span></span>|
|<span data-ttu-id="06920-151">id</span><span class="sxs-lookup"><span data-stu-id="06920-151">id</span></span>|<span data-ttu-id="06920-152">String</span><span class="sxs-lookup"><span data-stu-id="06920-152">String</span></span>| <span data-ttu-id="06920-153">A identificação do membro da equipe, em um formato GUID.</span><span class="sxs-lookup"><span data-stu-id="06920-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="06920-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06920-154">Read-only.</span></span>|
|<span data-ttu-id="06920-155">role</span><span class="sxs-lookup"><span data-stu-id="06920-155">role</span></span>|<span data-ttu-id="06920-156">string</span><span class="sxs-lookup"><span data-stu-id="06920-156">string</span></span>| <span data-ttu-id="06920-157">A função de membro da equipe de negócios.</span><span class="sxs-lookup"><span data-stu-id="06920-157">The role of the staff member in the business.</span></span> <span data-ttu-id="06920-158">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="06920-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="06920-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06920-159">Required.</span></span>|
|<span data-ttu-id="06920-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="06920-160">useBusinessHours</span></span>|<span data-ttu-id="06920-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="06920-161">Boolean</span></span>|<span data-ttu-id="06920-162">True significa disponibilidade do membro da equipe é como especificado na propriedade **businessHours** dos negócios.</span><span class="sxs-lookup"><span data-stu-id="06920-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="06920-163">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="06920-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="06920-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="06920-164">workingHours</span></span>|<span data-ttu-id="06920-165">coleção [bookingWorkHours](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="06920-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="06920-166">O intervalo de horas por dia da semana em que o membro da equipe está disponível para marcação.</span><span class="sxs-lookup"><span data-stu-id="06920-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="06920-167">Por padrão, eles são inicializados para ser o mesmo que a propriedade **businessHours** dos negócios.</span><span class="sxs-lookup"><span data-stu-id="06920-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06920-168">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="06920-168">Relationships</span></span>
<span data-ttu-id="06920-169">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06920-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="06920-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06920-170">JSON representation</span></span>

<span data-ttu-id="06920-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06920-171">The following is a JSON representation of the resource.</span></span>

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
