---
title: Atualizar bookingappointment
description: Atualiza as propriedades de um objeto bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e2af9b0a547ecea9895802d3f4ab4666a243ed9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441281"
---
# <a name="update-bookingappointment"></a><span data-ttu-id="0af3b-103">Atualizar bookingappointment</span><span class="sxs-lookup"><span data-stu-id="0af3b-103">Update bookingappointment</span></span>

<span data-ttu-id="0af3b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0af3b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af3b-105">Atualiza as propriedades de um objeto [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="0af3b-105">Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0af3b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0af3b-106">Permissions</span></span>
<span data-ttu-id="0af3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af3b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0af3b-109">Permission type</span></span>      | <span data-ttu-id="0af3b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0af3b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af3b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0af3b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0af3b-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="0af3b-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0af3b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0af3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af3b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0af3b-114">Not supported.</span></span>   |
|<span data-ttu-id="0af3b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0af3b-115">Application</span></span> | <span data-ttu-id="0af3b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0af3b-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0af3b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0af3b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0af3b-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0af3b-118">Optional request headers</span></span>
| <span data-ttu-id="0af3b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0af3b-119">Name</span></span>       | <span data-ttu-id="0af3b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0af3b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0af3b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af3b-121">Authorization</span></span>  | <span data-ttu-id="0af3b-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0af3b-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af3b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0af3b-123">Request body</span></span>
<span data-ttu-id="0af3b-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0af3b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0af3b-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0af3b-127">Property</span></span>     | <span data-ttu-id="0af3b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0af3b-128">Type</span></span>   |<span data-ttu-id="0af3b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0af3b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0af3b-130">customerEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0af3b-130">customerEmailAddress</span></span>|<span data-ttu-id="0af3b-131">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-131">String</span></span>|<span data-ttu-id="0af3b-132">O endereço SMTP do [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-132">The SMTP address of the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="0af3b-133">Box</span><span class="sxs-lookup"><span data-stu-id="0af3b-133">customerId</span></span>|<span data-ttu-id="0af3b-134">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-134">String</span></span>|<span data-ttu-id="0af3b-135">A ID do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-135">The ID of the [bookingCustomer](../resources/bookingcustomer.md) for this appointment.</span></span> <span data-ttu-id="0af3b-136">Se nenhuma ID for especificada quando um compromisso for criado, será criado um novo objeto **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="0af3b-136">If no ID is specified when an appointment is created, then a new **bookingCustomer** object is created.</span></span> <span data-ttu-id="0af3b-137">Depois de definido, considere o **CustomerID** imutável.</span><span class="sxs-lookup"><span data-stu-id="0af3b-137">Once set, you should consider the **customerId** immutable.</span></span>|
|<span data-ttu-id="0af3b-138">customerLocation</span><span class="sxs-lookup"><span data-stu-id="0af3b-138">customerLocation</span></span>|[<span data-ttu-id="0af3b-139">location</span><span class="sxs-lookup"><span data-stu-id="0af3b-139">location</span></span>](../resources/location.md)|<span data-ttu-id="0af3b-140">Representa as informações de local para o [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-140">Represents location information for the [bookingCustomer](../resources/bookingcustomer.md) who is booking the appointment.</span></span>|
|<span data-ttu-id="0af3b-141">Customer</span><span class="sxs-lookup"><span data-stu-id="0af3b-141">customerName</span></span>|<span data-ttu-id="0af3b-142">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-142">String</span></span>|<span data-ttu-id="0af3b-143">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="0af3b-143">The customer's name.</span></span>|
|<span data-ttu-id="0af3b-144">customerNotes</span><span class="sxs-lookup"><span data-stu-id="0af3b-144">customerNotes</span></span>|<span data-ttu-id="0af3b-145">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-145">String</span></span>|<span data-ttu-id="0af3b-146">Observações do cliente associado a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-146">Notes from the customer associated with this appointment.</span></span> <span data-ttu-id="0af3b-147">Você pode obter o valor somente ao ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="0af3b-147">You can get the value only when reading this **bookingAppointment** by its ID.</span></span> <br> <span data-ttu-id="0af3b-148">Você pode definir essa propriedade somente quando criar inicialmente um compromisso com um novo cliente.</span><span class="sxs-lookup"><span data-stu-id="0af3b-148">You can set this property only when initially creating an appointment with a new customer.</span></span> <span data-ttu-id="0af3b-149">Após esse ponto, o valor é calculado a partir do cliente representado por **CustomerID**.</span><span class="sxs-lookup"><span data-stu-id="0af3b-149">After that point, the value is computed from the customer represented by **customerId**.</span></span>|
|<span data-ttu-id="0af3b-150">customerPhone</span><span class="sxs-lookup"><span data-stu-id="0af3b-150">customerPhone</span></span>|<span data-ttu-id="0af3b-151">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-151">String</span></span>|<span data-ttu-id="0af3b-152">O número de telefone do cliente.</span><span class="sxs-lookup"><span data-stu-id="0af3b-152">The customer's phone number.</span></span>|
|<span data-ttu-id="0af3b-153">duration</span><span class="sxs-lookup"><span data-stu-id="0af3b-153">duration</span></span>|<span data-ttu-id="0af3b-154">Duração</span><span class="sxs-lookup"><span data-stu-id="0af3b-154">Duration</span></span>|<span data-ttu-id="0af3b-155">O comprimento do compromisso, indicado no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="0af3b-155">The length of the appointment, denoted in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="0af3b-156">end</span><span class="sxs-lookup"><span data-stu-id="0af3b-156">end</span></span>|[<span data-ttu-id="0af3b-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0af3b-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0af3b-158">A data, a hora e o fuso horário em que o compromisso termina.</span><span class="sxs-lookup"><span data-stu-id="0af3b-158">The date, time, and time zone that the appointment ends.</span></span>|
|<span data-ttu-id="0af3b-159">invoiceAmount</span><span class="sxs-lookup"><span data-stu-id="0af3b-159">invoiceAmount</span></span>|<span data-ttu-id="0af3b-160">Duplo</span><span class="sxs-lookup"><span data-stu-id="0af3b-160">Double</span></span>|<span data-ttu-id="0af3b-161">O valor cobrado na fatura.</span><span class="sxs-lookup"><span data-stu-id="0af3b-161">The billed amount on the invoice.</span></span>|
|<span data-ttu-id="0af3b-162">invoiceDate</span><span class="sxs-lookup"><span data-stu-id="0af3b-162">invoiceDate</span></span>|[<span data-ttu-id="0af3b-163">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0af3b-163">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0af3b-164">A data, a hora e o fuso horário da fatura para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-164">The date, time, and time zone of the invoice for this appointment.</span></span>|
|<span data-ttu-id="0af3b-165">faturaid</span><span class="sxs-lookup"><span data-stu-id="0af3b-165">invoiceId</span></span>|<span data-ttu-id="0af3b-166">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-166">String</span></span>|<span data-ttu-id="0af3b-167">A ID da fatura.</span><span class="sxs-lookup"><span data-stu-id="0af3b-167">The ID of the invoice.</span></span>|
|<span data-ttu-id="0af3b-168">invoiceStatus</span><span class="sxs-lookup"><span data-stu-id="0af3b-168">invoiceStatus</span></span>|<span data-ttu-id="0af3b-169">string</span><span class="sxs-lookup"><span data-stu-id="0af3b-169">string</span></span>| <span data-ttu-id="0af3b-170">O status da fatura.</span><span class="sxs-lookup"><span data-stu-id="0af3b-170">The status of the invoice.</span></span> <span data-ttu-id="0af3b-171">Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span><span class="sxs-lookup"><span data-stu-id="0af3b-171">Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.</span></span>|
|<span data-ttu-id="0af3b-172">invoiceUrl</span><span class="sxs-lookup"><span data-stu-id="0af3b-172">invoiceUrl</span></span>|<span data-ttu-id="0af3b-173">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-173">String</span></span>|<span data-ttu-id="0af3b-174">A URL da fatura em Microsoft bookings.</span><span class="sxs-lookup"><span data-stu-id="0af3b-174">The URL of the invoice in Microsoft Bookings.</span></span>|
|<span data-ttu-id="0af3b-175">optOutOfCustomerEmail</span><span class="sxs-lookup"><span data-stu-id="0af3b-175">optOutOfCustomerEmail</span></span>|<span data-ttu-id="0af3b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="0af3b-176">Boolean</span></span>|<span data-ttu-id="0af3b-177">True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação desse compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-177">True indicates that the [bookingCustomer](../resources/bookingcustomer.md) for this appointment does not wish to receive a confirmation for this appointment.</span></span>|
|<span data-ttu-id="0af3b-178">Buffer</span><span class="sxs-lookup"><span data-stu-id="0af3b-178">postBuffer</span></span>|<span data-ttu-id="0af3b-179">Duração</span><span class="sxs-lookup"><span data-stu-id="0af3b-179">Duration</span></span>|<span data-ttu-id="0af3b-180">A quantidade de tempo para reservar depois que o compromisso termina, para limpeza, como um exemplo.</span><span class="sxs-lookup"><span data-stu-id="0af3b-180">The amount of time to reserve after the appointment ends, for cleaning up, as an example.</span></span> <span data-ttu-id="0af3b-181">O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="0af3b-181">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span> |
|<span data-ttu-id="0af3b-182">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="0af3b-182">preBuffer</span></span>|<span data-ttu-id="0af3b-183">Duração</span><span class="sxs-lookup"><span data-stu-id="0af3b-183">Duration</span></span>|<span data-ttu-id="0af3b-184">A quantidade de tempo para reservar antes de o compromisso começar, para preparação, como um exemplo.</span><span class="sxs-lookup"><span data-stu-id="0af3b-184">The amount of time to reserve before the appointment begins, for preparation, as an example.</span></span> <span data-ttu-id="0af3b-185">O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .</span><span class="sxs-lookup"><span data-stu-id="0af3b-185">The value is expressed in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="0af3b-186">descontos</span><span class="sxs-lookup"><span data-stu-id="0af3b-186">price</span></span>|<span data-ttu-id="0af3b-187">Duplo</span><span class="sxs-lookup"><span data-stu-id="0af3b-187">Double</span></span>|<span data-ttu-id="0af3b-188">O preço regular de um compromisso para o [bookingService](../resources/bookingservice.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="0af3b-188">The regular price for an appointment for the specified [bookingService](../resources/bookingservice.md).</span></span>|
|<span data-ttu-id="0af3b-189">PriceType</span><span class="sxs-lookup"><span data-stu-id="0af3b-189">priceType</span></span>|<span data-ttu-id="0af3b-190">string</span><span class="sxs-lookup"><span data-stu-id="0af3b-190">string</span></span>| <span data-ttu-id="0af3b-191">Uma configuração para fornecer flexibilidade para a estrutura de preços de serviços.</span><span class="sxs-lookup"><span data-stu-id="0af3b-191">A setting to provide flexibility for the pricing structure of services.</span></span> <span data-ttu-id="0af3b-192">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="0af3b-192">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="0af3b-193">lembretes</span><span class="sxs-lookup"><span data-stu-id="0af3b-193">reminders</span></span>|<span data-ttu-id="0af3b-194">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="0af3b-194">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="0af3b-195">O conjunto de lembretes do cliente enviado para este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-195">The collection of customer reminders sent for this appointment.</span></span> <span data-ttu-id="0af3b-196">O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="0af3b-196">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="0af3b-197">selfServiceAppointmentId</span><span class="sxs-lookup"><span data-stu-id="0af3b-197">selfServiceAppointmentId</span></span>|<span data-ttu-id="0af3b-198">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-198">String</span></span>|<span data-ttu-id="0af3b-199">Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="0af3b-199">An additional tracking ID for the appointment, if the appointment has been created directly by the customer on the scheduling page, as opposed to by a staff member on the behalf of the customer.</span></span>|
|<span data-ttu-id="0af3b-200">serviceId</span><span class="sxs-lookup"><span data-stu-id="0af3b-200">serviceId</span></span>|<span data-ttu-id="0af3b-201">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-201">String</span></span>|<span data-ttu-id="0af3b-202">A ID da [bookingService](../resources/bookingservice.md) associada a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-202">The ID of the [bookingService](../resources/bookingservice.md) associated with this appointment.</span></span>|
|<span data-ttu-id="0af3b-203">serviceLocation</span><span class="sxs-lookup"><span data-stu-id="0af3b-203">serviceLocation</span></span>|[<span data-ttu-id="0af3b-204">location</span><span class="sxs-lookup"><span data-stu-id="0af3b-204">location</span></span>](../resources/location.md)|<span data-ttu-id="0af3b-205">O local onde o serviço é entregue.</span><span class="sxs-lookup"><span data-stu-id="0af3b-205">The location where the service is delivered.</span></span>|
|<span data-ttu-id="0af3b-206">serviceName</span><span class="sxs-lookup"><span data-stu-id="0af3b-206">serviceName</span></span>|<span data-ttu-id="0af3b-207">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-207">String</span></span>|<span data-ttu-id="0af3b-208">O nome do **bookingService** associado a este compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-208">The name of the **bookingService** associated with this appointment.</span></span><br><span data-ttu-id="0af3b-209">Essa propriedade é opcional ao criar um novo compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-209">This property is optional when creating a new appointment.</span></span> <span data-ttu-id="0af3b-210">Se não for especificado, será calculado a partir do serviço associado ao compromisso pela propriedade **ServiceId** .</span><span class="sxs-lookup"><span data-stu-id="0af3b-210">If not specified, it is computed from the service associated with the appointment by the **serviceId** property.</span></span>|
|<span data-ttu-id="0af3b-211">Notas</span><span class="sxs-lookup"><span data-stu-id="0af3b-211">serviceNotes</span></span>|<span data-ttu-id="0af3b-212">String</span><span class="sxs-lookup"><span data-stu-id="0af3b-212">String</span></span>|<span data-ttu-id="0af3b-213">Observações de um [bookingStaffMember](../resources/bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="0af3b-213">Notes from a [bookingStaffMember](../resources/bookingstaffmember.md).</span></span> <span data-ttu-id="0af3b-214">O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="0af3b-214">The value of this property is available only when reading this **bookingAppointment** by its ID.</span></span>|
|<span data-ttu-id="0af3b-215">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="0af3b-215">staffMemberIds</span></span>|<span data-ttu-id="0af3b-216">String collection</span><span class="sxs-lookup"><span data-stu-id="0af3b-216">String collection</span></span>|<span data-ttu-id="0af3b-217">A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) que está agendado neste compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-217">The ID of each [bookingStaffMember](../resources/bookingstaffmember.md) who is scheduled in this appointment.</span></span>|
|<span data-ttu-id="0af3b-218">iniciar</span><span class="sxs-lookup"><span data-stu-id="0af3b-218">start</span></span>|[<span data-ttu-id="0af3b-219">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0af3b-219">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0af3b-220">A data, a hora e o fuso horário de início do compromisso.</span><span class="sxs-lookup"><span data-stu-id="0af3b-220">The date, time, and time zone that the appointment begins.</span></span>|


## <a name="response"></a><span data-ttu-id="0af3b-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="0af3b-221">Response</span></span>
<span data-ttu-id="0af3b-p113">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0af3b-p113">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0af3b-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0af3b-224">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0af3b-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0af3b-225">Request</span></span>
<span data-ttu-id="0af3b-226">O exemplo a seguir altera a data de serviço por um dia e também atualiza a data da fatura.</span><span class="sxs-lookup"><span data-stu-id="0af3b-226">The following example changes the date of service by a day, and updated the invoice date as well.</span></span>

# <a name="http"></a>[<span data-ttu-id="0af3b-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af3b-227">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0af3b-228">C#</span><span class="sxs-lookup"><span data-stu-id="0af3b-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0af3b-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0af3b-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0af3b-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af3b-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0af3b-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="0af3b-231">Response</span></span>
<span data-ttu-id="0af3b-232">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0af3b-232">The following is an example of the response.</span></span>
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
