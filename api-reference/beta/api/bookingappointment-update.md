---
title: Atualizar bookingappointment
description: Atualiza as propriedades de um objeto bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: abdb15ea5b27071854bf8ece09d037e5d2e95fdb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945223"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="5c01e-103">Atualizar bookingappointment</span><span class="sxs-lookup"><span data-stu-id="5c01e-103">Update bookingappointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c01e-104">Atualiza as propriedades de um objeto [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="5c01e-104">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5c01e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c01e-105">Permissions</span></span>
<span data-ttu-id="5c01e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c01e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c01e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c01e-108">Permission type</span></span>      | <span data-ttu-id="5c01e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c01e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c01e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c01e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5c01e-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="5c01e-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5c01e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c01e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c01e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c01e-113">Not supported.</span></span>   |
|<span data-ttu-id="5c01e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c01e-114">Application</span></span> | <span data-ttu-id="5c01e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c01e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5c01e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c01e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5c01e-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="5c01e-117">Optional request headers</span></span>
| <span data-ttu-id="5c01e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5c01e-118">Name</span></span>       | <span data-ttu-id="5c01e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c01e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5c01e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c01e-120">Authorization</span></span>  | <span data-ttu-id="5c01e-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5c01e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c01e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c01e-122">Request body</span></span>
<span data-ttu-id="5c01e-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5c01e-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5c01e-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c01e-126">Property</span></span>     | <span data-ttu-id="5c01e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c01e-127">Type</span></span>   |<span data-ttu-id="5c01e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c01e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c01e-129">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5c01e-129">customerEmailAddress</span></span>|<span data-ttu-id="5c01e-130">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-130">String</span></span>|<span data-ttu-id="5c01e-131">O endereço SMTP do [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-131">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="5c01e-132">Box</span><span class="sxs-lookup"><span data-stu-id="5c01e-132">customerId</span></span>|<span data-ttu-id="5c01e-133">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-133">String</span></span>|<span data-ttu-id="5c01e-134">A ID do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-134">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="5c01e-135">Se nenhuma ID for especificada quando um compromisso for criado, será criado um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="5c01e-135">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="5c01e-136">Depois de definido, considere o **CustomerID** imutável.</span><span class="sxs-lookup"><span data-stu-id="5c01e-136">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="5c01e-137">customerLocation</span><span class="sxs-lookup"><span data-stu-id="5c01e-137">customerLocation</span></span>|[<span data-ttu-id="5c01e-138">location</span><span class="sxs-lookup"><span data-stu-id="5c01e-138">location</span></span>](../resources/location.md)|<span data-ttu-id="5c01e-139">Representa as informações de local para o [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-139">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="5c01e-140">Customer</span><span class="sxs-lookup"><span data-stu-id="5c01e-140">customerName</span></span>|<span data-ttu-id="5c01e-141">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-141">String</span></span>|<span data-ttu-id="5c01e-142">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="5c01e-142">The customer's name.</span></span>|
|<span data-ttu-id="5c01e-143">customerNotes</span><span class="sxs-lookup"><span data-stu-id="5c01e-143">customerNotes</span></span>|<span data-ttu-id="5c01e-144">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-144">String</span></span>|<span data-ttu-id="5c01e-145">Observações do cliente associado a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-145">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="5c01e-146">Você pode obter o valor somente ao ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="5c01e-146">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="5c01e-147">Você pode definir essa propriedade somente quando criar inicialmente um compromisso com um novo cliente.</span><span class="sxs-lookup"><span data-stu-id="5c01e-147">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="5c01e-148">Após esse ponto, o valor é calculado a partir do cliente representado por **CustomerID**.</span><span class="sxs-lookup"><span data-stu-id="5c01e-148">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="5c01e-149">customerPhone</span><span class="sxs-lookup"><span data-stu-id="5c01e-149">customerPhone</span></span>|<span data-ttu-id="5c01e-150">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-150">String</span></span>|<span data-ttu-id="5c01e-151">O número de telefone do cliente.</span><span class="sxs-lookup"><span data-stu-id="5c01e-151">The customer's phone number.</span></span>|
|<span data-ttu-id="5c01e-152">duration</span><span class="sxs-lookup"><span data-stu-id="5c01e-152">duration</span></span>|<span data-ttu-id="5c01e-153">Duração</span><span class="sxs-lookup"><span data-stu-id="5c01e-153">Duration</span></span>|<span data-ttu-id="5c01e-154">O comprimento do compromisso, indicado no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5c01e-154">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="5c01e-155">end</span><span class="sxs-lookup"><span data-stu-id="5c01e-155">end</span></span>|[<span data-ttu-id="5c01e-156">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c01e-156">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5c01e-157">A data, a hora e o fuso horário em que o compromisso termina.</span><span class="sxs-lookup"><span data-stu-id="5c01e-157">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="5c01e-158">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="5c01e-158">invoiceAmount</span></span>|<span data-ttu-id="5c01e-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="5c01e-159">Double</span></span>|<span data-ttu-id="5c01e-160">O valor cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="5c01e-160">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="5c01e-161">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="5c01e-161">invoiceDate</span></span>|[<span data-ttu-id="5c01e-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c01e-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5c01e-163">A data, a hora e o fuso horário da fatura para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-163">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="5c01e-164">faturaid</span><span class="sxs-lookup"><span data-stu-id="5c01e-164">invoiceId</span></span>|<span data-ttu-id="5c01e-165">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-165">String</span></span>|<span data-ttu-id="5c01e-166">A ID da fatura.</span><span class="sxs-lookup"><span data-stu-id="5c01e-166">The ID of the invoice.</span></span>|
|<span data-ttu-id="5c01e-167">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="5c01e-167">invoiceStatus</span></span>|<span data-ttu-id="5c01e-168">string</span><span class="sxs-lookup"><span data-stu-id="5c01e-168">string</span></span>| <span data-ttu-id="5c01e-169">O status da fatura.</span><span class="sxs-lookup"><span data-stu-id="5c01e-169">The status of the invoice.</span></span> <span data-ttu-id="5c01e-170">Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="5c01e-170">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="5c01e-171">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="5c01e-171">invoiceUrl</span></span>|<span data-ttu-id="5c01e-172">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-172">String</span></span>|<span data-ttu-id="5c01e-173">A URL da fatura em Microsoft bookings.</span><span class="sxs-lookup"><span data-stu-id="5c01e-173">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="5c01e-174">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="5c01e-174">optOutOfCustomerEmail</span></span>|<span data-ttu-id="5c01e-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c01e-175">Boolean</span></span>|<span data-ttu-id="5c01e-176">True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação desse compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-176">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="5c01e-177">Buffer</span><span class="sxs-lookup"><span data-stu-id="5c01e-177">postBuffer</span></span>|<span data-ttu-id="5c01e-178">Duração</span><span class="sxs-lookup"><span data-stu-id="5c01e-178">Duration</span></span>|<span data-ttu-id="5c01e-179">A quantidade de tempo para reservar depois que o compromisso termina, para limpeza, como um exemplo.</span><span class="sxs-lookup"><span data-stu-id="5c01e-179">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="5c01e-180">O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5c01e-180">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="5c01e-181">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="5c01e-181">preBuffer</span></span>|<span data-ttu-id="5c01e-182">Duração</span><span class="sxs-lookup"><span data-stu-id="5c01e-182">Duration</span></span>|<span data-ttu-id="5c01e-183">A quantidade de tempo para reservar antes de o compromisso começar, para preparação, como um exemplo.</span><span class="sxs-lookup"><span data-stu-id="5c01e-183">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="5c01e-184">O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="5c01e-184">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="5c01e-185">descontos</span><span class="sxs-lookup"><span data-stu-id="5c01e-185">price</span></span>|<span data-ttu-id="5c01e-186">Duplo</span><span class="sxs-lookup"><span data-stu-id="5c01e-186">Double</span></span>|<span data-ttu-id="5c01e-187">O preço regular de um compromisso para o [bookingService](../resources/bookingservice.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="5c01e-187">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="5c01e-188">PriceType</span><span class="sxs-lookup"><span data-stu-id="5c01e-188">priceType</span></span>|<span data-ttu-id="5c01e-189">string</span><span class="sxs-lookup"><span data-stu-id="5c01e-189">string</span></span>| <span data-ttu-id="5c01e-190">Uma configuração para fornecer flexibilidade para a estrutura de preços de serviços.</span><span class="sxs-lookup"><span data-stu-id="5c01e-190">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="5c01e-191">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="5c01e-191">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="5c01e-192">lembretes</span><span class="sxs-lookup"><span data-stu-id="5c01e-192">reminders</span></span>|<span data-ttu-id="5c01e-193">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="5c01e-193">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="5c01e-194">O conjunto de lembretes do cliente enviado para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-194">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="5c01e-195">O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="5c01e-195">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="5c01e-196">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="5c01e-196">selfServiceAppointmentId</span></span>|<span data-ttu-id="5c01e-197">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-197">String</span></span>|<span data-ttu-id="5c01e-198">Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="5c01e-198">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="5c01e-199">serviceId</span><span class="sxs-lookup"><span data-stu-id="5c01e-199">serviceId</span></span>|<span data-ttu-id="5c01e-200">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-200">String</span></span>|<span data-ttu-id="5c01e-201">A ID da [bookingService](../resources/bookingservice.md) associada a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-201">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="5c01e-202">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="5c01e-202">serviceLocation</span></span>|[<span data-ttu-id="5c01e-203">location</span><span class="sxs-lookup"><span data-stu-id="5c01e-203">location</span></span>](../resources/location.md)|<span data-ttu-id="5c01e-204">O local onde o serviço é entregue.</span><span class="sxs-lookup"><span data-stu-id="5c01e-204">The location where the service is delivered.</span></span>|
|<span data-ttu-id="5c01e-205">serviceName</span><span class="sxs-lookup"><span data-stu-id="5c01e-205">serviceName</span></span>|<span data-ttu-id="5c01e-206">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-206">String</span></span>|<span data-ttu-id="5c01e-207">O nome do **bookingService** associado a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-207">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="5c01e-208">Essa propriedade é opcional ao criar um novo compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-208">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="5c01e-209">Se não for especificado, será calculado a partir do serviço associado ao compromisso pela propriedade **ServiceId** .</span><span class="sxs-lookup"><span data-stu-id="5c01e-209">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="5c01e-210">Notas</span><span class="sxs-lookup"><span data-stu-id="5c01e-210">serviceNotes</span></span>|<span data-ttu-id="5c01e-211">String</span><span class="sxs-lookup"><span data-stu-id="5c01e-211">String</span></span>|<span data-ttu-id="5c01e-212">Observações de um [bookingStaffMember](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="5c01e-212">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="5c01e-213">O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="5c01e-213">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="5c01e-214">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="5c01e-214">staffMemberIds</span></span>|<span data-ttu-id="5c01e-215">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c01e-215">String collection</span></span>|<span data-ttu-id="5c01e-216">A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) que está agendado neste compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-216">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="5c01e-217">iniciar</span><span class="sxs-lookup"><span data-stu-id="5c01e-217">start</span></span>|[<span data-ttu-id="5c01e-218">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5c01e-218">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="5c01e-219">A data, a hora e o fuso horário de início do compromisso.</span><span class="sxs-lookup"><span data-stu-id="5c01e-219">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="5c01e-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c01e-220">Response</span></span>
<span data-ttu-id="5c01e-p113">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c01e-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c01e-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c01e-223">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c01e-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c01e-224">Request</span></span>
<span data-ttu-id="5c01e-225">O exemplo a seguir altera a data de serviço por um dia e também atualiza a data da fatura.</span><span class="sxs-lookup"><span data-stu-id="5c01e-225">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5c01e-226">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c01e-226">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5c01e-227">C#</span><span class="sxs-lookup"><span data-stu-id="5c01e-227">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5c01e-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="5c01e-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5c01e-229">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5c01e-229">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5c01e-230">Java</span><span class="sxs-lookup"><span data-stu-id="5c01e-230">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c01e-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c01e-231">Response</span></span>
<span data-ttu-id="5c01e-232">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c01e-232">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
