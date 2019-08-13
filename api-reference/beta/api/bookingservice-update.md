---
title: Atualizar bookingservice
description: Atualiza as propriedades de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b687a0f84cf3433c8d8e0d42f0e362e1b6f30e9a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318086"
---
# <a name="update-bookingservice"></a><span data-ttu-id="055c7-103">Atualizar bookingservice</span><span class="sxs-lookup"><span data-stu-id="055c7-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="055c7-104">Atualiza as propriedades de um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="055c7-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="055c7-105">Veja a seguir alguns exemplos que você pode personalizar para um serviço:</span><span class="sxs-lookup"><span data-stu-id="055c7-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="055c7-106">Price</span><span class="sxs-lookup"><span data-stu-id="055c7-106">Price</span></span>
- <span data-ttu-id="055c7-107">Tamanho típico de um compromisso</span><span class="sxs-lookup"><span data-stu-id="055c7-107">Typical length of an appointment</span></span>
- <span data-ttu-id="055c7-108">Lembretes</span><span class="sxs-lookup"><span data-stu-id="055c7-108">Reminders</span></span>
- <span data-ttu-id="055c7-109">Qualquer buffer de tempo a ser configurado antes ou termine após o serviço</span><span class="sxs-lookup"><span data-stu-id="055c7-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="055c7-110">Parâmetros de [política de agendamento](../resources/bookingschedulingpolicy.md) , como o aviso mínimo, para livro ou cancelamento, e se os clientes podem selecionar membros específicos da equipe para um compromisso.</span><span class="sxs-lookup"><span data-stu-id="055c7-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="055c7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="055c7-111">Permissions</span></span>
<span data-ttu-id="055c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="055c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="055c7-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="055c7-114">Permission type</span></span>      | <span data-ttu-id="055c7-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="055c7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="055c7-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="055c7-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="055c7-117">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="055c7-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="055c7-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="055c7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="055c7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="055c7-119">Not supported.</span></span>   |
|<span data-ttu-id="055c7-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="055c7-120">Application</span></span> | <span data-ttu-id="055c7-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="055c7-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="055c7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="055c7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="055c7-123">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="055c7-123">Optional request headers</span></span>
| <span data-ttu-id="055c7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="055c7-124">Name</span></span>       | <span data-ttu-id="055c7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="055c7-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="055c7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="055c7-126">Authorization</span></span>  | <span data-ttu-id="055c7-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="055c7-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="055c7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="055c7-128">Request body</span></span>
<span data-ttu-id="055c7-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="055c7-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="055c7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="055c7-132">Property</span></span>     | <span data-ttu-id="055c7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="055c7-133">Type</span></span>   |<span data-ttu-id="055c7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="055c7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="055c7-135">defaultduration</span><span class="sxs-lookup"><span data-stu-id="055c7-135">defaultDuration</span></span>|<span data-ttu-id="055c7-136">Duração</span><span class="sxs-lookup"><span data-stu-id="055c7-136">Duration</span></span>|<span data-ttu-id="055c7-137">O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos.</span><span class="sxs-lookup"><span data-stu-id="055c7-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="055c7-138">Por exemplo, P11D23H59M 59.999999999999 S.</span><span class="sxs-lookup"><span data-stu-id="055c7-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="055c7-139">DefaultLocation</span><span class="sxs-lookup"><span data-stu-id="055c7-139">defaultLocation</span></span>|[<span data-ttu-id="055c7-140">location</span><span class="sxs-lookup"><span data-stu-id="055c7-140">location</span></span>](../resources/location.md)|<span data-ttu-id="055c7-141">O local físico padrão para o serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="055c7-142">defaultprice</span><span class="sxs-lookup"><span data-stu-id="055c7-142">defaultPrice</span></span>|<span data-ttu-id="055c7-143">Duplo</span><span class="sxs-lookup"><span data-stu-id="055c7-143">Double</span></span>|<span data-ttu-id="055c7-144">O preço monetário padrão do serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="055c7-145">defaultpricetype</span><span class="sxs-lookup"><span data-stu-id="055c7-145">defaultPriceType</span></span>|<span data-ttu-id="055c7-146">string</span><span class="sxs-lookup"><span data-stu-id="055c7-146">string</span></span>|<span data-ttu-id="055c7-147">O modo padrão pelo qual o serviço é cobrado.</span><span class="sxs-lookup"><span data-stu-id="055c7-147">The default way the service is charged.</span></span> <span data-ttu-id="055c7-148">Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="055c7-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="055c7-149">defaultlembrers</span><span class="sxs-lookup"><span data-stu-id="055c7-149">defaultReminders</span></span>|<span data-ttu-id="055c7-150">coleção [bookingReminder](../resources/bookingreminder.md)</span><span class="sxs-lookup"><span data-stu-id="055c7-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="055c7-151">O conjunto padrão de lembretes para um compromisso desse serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="055c7-152">O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.</span><span class="sxs-lookup"><span data-stu-id="055c7-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="055c7-153">descrição</span><span class="sxs-lookup"><span data-stu-id="055c7-153">description</span></span>|<span data-ttu-id="055c7-154">String</span><span class="sxs-lookup"><span data-stu-id="055c7-154">String</span></span>|<span data-ttu-id="055c7-155">Uma descrição de texto para o serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-155">A text description for the service.</span></span>|
|<span data-ttu-id="055c7-156">displayName</span><span class="sxs-lookup"><span data-stu-id="055c7-156">displayName</span></span>|<span data-ttu-id="055c7-157">String</span><span class="sxs-lookup"><span data-stu-id="055c7-157">String</span></span>|<span data-ttu-id="055c7-158">Um nome de serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-158">A service name.</span></span>|
|<span data-ttu-id="055c7-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="055c7-159">emailAddress</span></span>|<span data-ttu-id="055c7-160">String</span><span class="sxs-lookup"><span data-stu-id="055c7-160">String</span></span>|<span data-ttu-id="055c7-161">Um endereço de email</span><span class="sxs-lookup"><span data-stu-id="055c7-161">An email address</span></span>|
|<span data-ttu-id="055c7-162">id</span><span class="sxs-lookup"><span data-stu-id="055c7-162">id</span></span>|<span data-ttu-id="055c7-163">String</span><span class="sxs-lookup"><span data-stu-id="055c7-163">String</span></span>| <span data-ttu-id="055c7-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="055c7-164">Read-only.</span></span>|
|<span data-ttu-id="055c7-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="055c7-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="055c7-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="055c7-166">Boolean</span></span>|<span data-ttu-id="055c7-167">True significa que este serviço não está disponível para os clientes para reserva.</span><span class="sxs-lookup"><span data-stu-id="055c7-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="055c7-168">notes</span><span class="sxs-lookup"><span data-stu-id="055c7-168">notes</span></span>|<span data-ttu-id="055c7-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="055c7-169">String</span></span>|<span data-ttu-id="055c7-170">Informações adicionais sobre este serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-170">Additional information about this service.</span></span>|
|<span data-ttu-id="055c7-171">Buffer</span><span class="sxs-lookup"><span data-stu-id="055c7-171">postBuffer</span></span>|<span data-ttu-id="055c7-172">Duração</span><span class="sxs-lookup"><span data-stu-id="055c7-172">Duration</span></span>|<span data-ttu-id="055c7-173">O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.</span><span class="sxs-lookup"><span data-stu-id="055c7-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="055c7-174">antes do buffer</span><span class="sxs-lookup"><span data-stu-id="055c7-174">preBuffer</span></span>|<span data-ttu-id="055c7-175">Duração</span><span class="sxs-lookup"><span data-stu-id="055c7-175">Duration</span></span>|<span data-ttu-id="055c7-176">O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.</span><span class="sxs-lookup"><span data-stu-id="055c7-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="055c7-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="055c7-177">schedulingPolicy</span></span>|[<span data-ttu-id="055c7-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="055c7-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="055c7-179">O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.</span><span class="sxs-lookup"><span data-stu-id="055c7-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="055c7-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="055c7-180">staffMemberIds</span></span>|<span data-ttu-id="055c7-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="055c7-181">String collection</span></span>|<span data-ttu-id="055c7-182">Representa os [membros da equipe](../resources/bookingstaffmember.md) que fornecem esse serviço.</span><span class="sxs-lookup"><span data-stu-id="055c7-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="055c7-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="055c7-183">Response</span></span>
<span data-ttu-id="055c7-p106">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="055c7-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="055c7-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="055c7-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="055c7-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="055c7-187">Request</span></span>
<span data-ttu-id="055c7-188">O exemplo a seguir atualiza a duração do serviço especificado.</span><span class="sxs-lookup"><span data-stu-id="055c7-188">The following example updates the duration of the specified service.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="055c7-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="055c7-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="055c7-190">C#</span><span class="sxs-lookup"><span data-stu-id="055c7-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="055c7-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="055c7-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="055c7-192">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="055c7-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="055c7-193">Java</span><span class="sxs-lookup"><span data-stu-id="055c7-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="055c7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="055c7-194">Response</span></span>
<span data-ttu-id="055c7-195">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="055c7-195">The following is an example of the response.</span></span>
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
