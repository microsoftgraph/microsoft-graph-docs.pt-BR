---
title: Atualizar bookingservice
description: Atualiza as propriedades de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 15ed5e3a922fe4e630287c6193ff1daa8822fb30
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987852"
---
# <a name="update-bookingservice"></a><span data-ttu-id="276d2-103">Atualizar bookingservice</span><span class="sxs-lookup"><span data-stu-id="276d2-103">Update bookingservice</span></span>

<span data-ttu-id="276d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="276d2-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="276d2-105">Atualiza as propriedades de um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="276d2-105">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="276d2-106">Veja a seguir alguns exemplos que você pode personalizar para um serviço:</span><span class="sxs-lookup"><span data-stu-id="276d2-106">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="276d2-107">Price</span><span class="sxs-lookup"><span data-stu-id="276d2-107">Price</span></span>
- <span data-ttu-id="276d2-108">Tamanho típico de um compromisso</span><span class="sxs-lookup"><span data-stu-id="276d2-108">Typical length of an appointment</span></span>
- <span data-ttu-id="276d2-109">Reminders</span><span class="sxs-lookup"><span data-stu-id="276d2-109">Reminders</span></span>
- <span data-ttu-id="276d2-110">Qualquer buffer de tempo a ser configurado antes ou termine após o serviço</span><span class="sxs-lookup"><span data-stu-id="276d2-110">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="276d2-111">Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como o aviso mínimo, para livro ou cancelamento, e se os clientes podem selecionar membros específicos da equipe para um compromisso.</span><span class="sxs-lookup"><span data-stu-id="276d2-111">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="276d2-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="276d2-112">Permissions</span></span>
<span data-ttu-id="276d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="276d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="276d2-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="276d2-115">Permission type</span></span>      | <span data-ttu-id="276d2-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="276d2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="276d2-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="276d2-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="276d2-118">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="276d2-118">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="276d2-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="276d2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="276d2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276d2-120">Not supported.</span></span>   |
|<span data-ttu-id="276d2-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="276d2-121">Application</span></span> | <span data-ttu-id="276d2-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="276d2-122">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="276d2-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="276d2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="276d2-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="276d2-124">Optional request headers</span></span>
| <span data-ttu-id="276d2-125">Nome</span><span class="sxs-lookup"><span data-stu-id="276d2-125">Name</span></span>       | <span data-ttu-id="276d2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="276d2-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="276d2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="276d2-127">Authorization</span></span>  | <span data-ttu-id="276d2-128">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="276d2-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="276d2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="276d2-129">Request body</span></span>
<span data-ttu-id="276d2-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="276d2-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="276d2-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="276d2-133">Property</span></span>     | <span data-ttu-id="276d2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="276d2-134">Type</span></span>   |<span data-ttu-id="276d2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="276d2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="276d2-136">defaultduration</span><span class="sxs-lookup"><span data-stu-id="276d2-136">defaultDuration</span></span>|<span data-ttu-id="276d2-137">Duração</span><span class="sxs-lookup"><span data-stu-id="276d2-137">Duration</span></span>|<span data-ttu-id="276d2-138">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="276d2-138">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="276d2-139">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="276d2-139">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="276d2-140">DefaultLocation</span><span class="sxs-lookup"><span data-stu-id="276d2-140">defaultLocation</span></span>|[<span data-ttu-id="276d2-141">location</span><span class="sxs-lookup"><span data-stu-id="276d2-141">location</span></span>](../resources/location.md)|<span data-ttu-id="276d2-142">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-142">The default physical location for the service.</span></span>|
|<span data-ttu-id="276d2-143">defaultprice</span><span class="sxs-lookup"><span data-stu-id="276d2-143">defaultPrice</span></span>|<span data-ttu-id="276d2-144">Duplo</span><span class="sxs-lookup"><span data-stu-id="276d2-144">Double</span></span>|<span data-ttu-id="276d2-145">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-145">The default monetary price for the service.</span></span>|
|<span data-ttu-id="276d2-146">defaultpricetype</span><span class="sxs-lookup"><span data-stu-id="276d2-146">defaultPriceType</span></span>|<span data-ttu-id="276d2-147">string</span><span class="sxs-lookup"><span data-stu-id="276d2-147">string</span></span>|<span data-ttu-id="276d2-148">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="276d2-148">The default way the service is charged.</span></span> <span data-ttu-id="276d2-149">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="276d2-149">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="276d2-150">defaultlembrers</span><span class="sxs-lookup"><span data-stu-id="276d2-150">defaultReminders</span></span>|<span data-ttu-id="276d2-151">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="276d2-151">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="276d2-152">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-152">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="276d2-153">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="276d2-153">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="276d2-154">description</span><span class="sxs-lookup"><span data-stu-id="276d2-154">description</span></span>|<span data-ttu-id="276d2-155">String</span><span class="sxs-lookup"><span data-stu-id="276d2-155">String</span></span>|<span data-ttu-id="276d2-156">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-156">A text description for the service.</span></span>|
|<span data-ttu-id="276d2-157">displayName</span><span class="sxs-lookup"><span data-stu-id="276d2-157">displayName</span></span>|<span data-ttu-id="276d2-158">String</span><span class="sxs-lookup"><span data-stu-id="276d2-158">String</span></span>|<span data-ttu-id="276d2-159">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-159">A service name.</span></span>|
|<span data-ttu-id="276d2-160">emailAddress</span><span class="sxs-lookup"><span data-stu-id="276d2-160">emailAddress</span></span>|<span data-ttu-id="276d2-161">String</span><span class="sxs-lookup"><span data-stu-id="276d2-161">String</span></span>|<span data-ttu-id="276d2-162">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="276d2-162">An email address</span></span>|
|<span data-ttu-id="276d2-163">id</span><span class="sxs-lookup"><span data-stu-id="276d2-163">id</span></span>|<span data-ttu-id="276d2-164">String</span><span class="sxs-lookup"><span data-stu-id="276d2-164">String</span></span>| <span data-ttu-id="276d2-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="276d2-165">Read-only.</span></span>|
|<span data-ttu-id="276d2-166">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="276d2-166">isHiddenFromCustomers</span></span>|<span data-ttu-id="276d2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="276d2-167">Boolean</span></span>|<span data-ttu-id="276d2-168">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="276d2-168">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="276d2-169">notes</span><span class="sxs-lookup"><span data-stu-id="276d2-169">notes</span></span>|<span data-ttu-id="276d2-170">String</span><span class="sxs-lookup"><span data-stu-id="276d2-170">String</span></span>|<span data-ttu-id="276d2-171">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-171">Additional information about this service.</span></span>|
|<span data-ttu-id="276d2-172">Buffer</span><span class="sxs-lookup"><span data-stu-id="276d2-172">postBuffer</span></span>|<span data-ttu-id="276d2-173">Duração</span><span class="sxs-lookup"><span data-stu-id="276d2-173">Duration</span></span>|<span data-ttu-id="276d2-174">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="276d2-174">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="276d2-175">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="276d2-175">preBuffer</span></span>|<span data-ttu-id="276d2-176">Duração</span><span class="sxs-lookup"><span data-stu-id="276d2-176">Duration</span></span>|<span data-ttu-id="276d2-177">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="276d2-177">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="276d2-178">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="276d2-178">schedulingPolicy</span></span>|[<span data-ttu-id="276d2-179">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="276d2-179">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="276d2-180">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="276d2-180">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="276d2-181">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="276d2-181">staffMemberIds</span></span>|<span data-ttu-id="276d2-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="276d2-182">String collection</span></span>|<span data-ttu-id="276d2-183">Representa os [membros da equipe](../resources/bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="276d2-183">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="276d2-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="276d2-184">Response</span></span>
<span data-ttu-id="276d2-p106">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="276d2-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="276d2-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="276d2-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="276d2-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="276d2-188">Request</span></span>
<span data-ttu-id="276d2-189">O exemplo a seguir atualiza a duração do serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="276d2-189">The following example updates the duration of the specified service.</span></span>

# <a name="http"></a>[<span data-ttu-id="276d2-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="276d2-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
# <a name="c"></a>[<span data-ttu-id="276d2-191">C#</span><span class="sxs-lookup"><span data-stu-id="276d2-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="276d2-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="276d2-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="276d2-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="276d2-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="276d2-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="276d2-194">Response</span></span>
<span data-ttu-id="276d2-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="276d2-195">The following is an example of the response.</span></span>
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


