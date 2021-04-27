---
title: Atualizar bookingbusiness
description: Atualize as propriedades de um objeto bookingBusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 767d4b3a355c74f6941bd9d9d20579e1c0dcda23
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047844"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="7a6eb-103">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="7a6eb-103">Update bookingbusiness</span></span>

<span data-ttu-id="7a6eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a6eb-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a6eb-105">Atualize as propriedades de um [objeto bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="7a6eb-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a6eb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a6eb-106">Permissions</span></span>
<span data-ttu-id="7a6eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a6eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a6eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a6eb-109">Permission type</span></span>      | <span data-ttu-id="7a6eb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a6eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a6eb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a6eb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="7a6eb-112">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7a6eb-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7a6eb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a6eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a6eb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-114">Not supported.</span></span>   |
|<span data-ttu-id="7a6eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a6eb-115">Application</span></span> | <span data-ttu-id="7a6eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7a6eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a6eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="7a6eb-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="7a6eb-118">Optional request headers</span></span>
| <span data-ttu-id="7a6eb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a6eb-119">Name</span></span>       | <span data-ttu-id="7a6eb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a6eb-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7a6eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a6eb-121">Authorization</span></span>  | <span data-ttu-id="7a6eb-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7a6eb-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a6eb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a6eb-123">Request body</span></span>
<span data-ttu-id="7a6eb-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7a6eb-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a6eb-127">Property</span></span>     | <span data-ttu-id="7a6eb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a6eb-128">Type</span></span>   |<span data-ttu-id="7a6eb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a6eb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a6eb-130">address</span><span class="sxs-lookup"><span data-stu-id="7a6eb-130">address</span></span>|[<span data-ttu-id="7a6eb-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7a6eb-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="7a6eb-132">O endereço da rua do negócio.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-132">The street address of the business.</span></span>|
|<span data-ttu-id="7a6eb-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="7a6eb-133">businessHours</span></span>|<span data-ttu-id="7a6eb-134">[Coleção bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="7a6eb-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="7a6eb-135">Os horários de operação para os negócios.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="7a6eb-136">businessType</span><span class="sxs-lookup"><span data-stu-id="7a6eb-136">businessType</span></span>|<span data-ttu-id="7a6eb-137">String</span><span class="sxs-lookup"><span data-stu-id="7a6eb-137">String</span></span>|<span data-ttu-id="7a6eb-138">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-138">The type of business.</span></span>|
|<span data-ttu-id="7a6eb-139">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="7a6eb-139">defaultCurrencyIso</span></span>|<span data-ttu-id="7a6eb-140">String</span><span class="sxs-lookup"><span data-stu-id="7a6eb-140">String</span></span>|<span data-ttu-id="7a6eb-141">O código da moeda em que a empresa opera no Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="7a6eb-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7a6eb-142">displayName</span></span>|<span data-ttu-id="7a6eb-143">String</span><span class="sxs-lookup"><span data-stu-id="7a6eb-143">String</span></span>|<span data-ttu-id="7a6eb-144">Um nome para a empresa que faz interface com os clientes.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="7a6eb-145">email</span><span class="sxs-lookup"><span data-stu-id="7a6eb-145">email</span></span>|<span data-ttu-id="7a6eb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a6eb-146">String</span></span>|<span data-ttu-id="7a6eb-147">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-147">The email address for the business.</span></span>|
|<span data-ttu-id="7a6eb-148">phone</span><span class="sxs-lookup"><span data-stu-id="7a6eb-148">phone</span></span>|<span data-ttu-id="7a6eb-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a6eb-149">String</span></span>|<span data-ttu-id="7a6eb-150">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="7a6eb-151">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7a6eb-151">schedulingPolicy</span></span>|[<span data-ttu-id="7a6eb-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="7a6eb-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="7a6eb-153">Especifica como as reservas podem ser criadas para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="7a6eb-154">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="7a6eb-154">webSiteUrl</span></span>|<span data-ttu-id="7a6eb-155">String</span><span class="sxs-lookup"><span data-stu-id="7a6eb-155">String</span></span>|<span data-ttu-id="7a6eb-156">A URL do site comercial.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="7a6eb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a6eb-157">Response</span></span>
<span data-ttu-id="7a6eb-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a6eb-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a6eb-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a6eb-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a6eb-161">Request</span></span>
<span data-ttu-id="7a6eb-162">O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão da empresa para uma hora e avançar a reserva até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a6eb-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a6eb-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="7a6eb-164">C#</span><span class="sxs-lookup"><span data-stu-id="7a6eb-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a6eb-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a6eb-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a6eb-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a6eb-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a6eb-167">Java</span><span class="sxs-lookup"><span data-stu-id="7a6eb-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a6eb-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a6eb-168">Response</span></span>
<span data-ttu-id="7a6eb-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-169">The following is an example of the response.</span></span> <span data-ttu-id="7a6eb-170">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a6eb-170">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


