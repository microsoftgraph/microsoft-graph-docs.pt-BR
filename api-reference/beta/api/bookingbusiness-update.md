---
title: Atualizar bookingbusiness
description: Atualiza as propriedades de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 377c1eb6bdbc0595e43785db8b31f08e4c2b2cb7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318205"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="8dce5-103">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="8dce5-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dce5-104">Atualiza as propriedades de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="8dce5-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8dce5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dce5-105">Permissions</span></span>
<span data-ttu-id="8dce5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dce5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dce5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dce5-108">Permission type</span></span>      | <span data-ttu-id="8dce5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dce5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dce5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dce5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8dce5-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="8dce5-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8dce5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dce5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dce5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dce5-113">Not supported.</span></span>   |
|<span data-ttu-id="8dce5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dce5-114">Application</span></span> | <span data-ttu-id="8dce5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dce5-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8dce5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dce5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="8dce5-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="8dce5-117">Optional request headers</span></span>
| <span data-ttu-id="8dce5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8dce5-118">Name</span></span>       | <span data-ttu-id="8dce5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dce5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8dce5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dce5-120">Authorization</span></span>  | <span data-ttu-id="8dce5-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8dce5-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dce5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dce5-122">Request body</span></span>
<span data-ttu-id="8dce5-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8dce5-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8dce5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dce5-126">Property</span></span>     | <span data-ttu-id="8dce5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dce5-127">Type</span></span>   |<span data-ttu-id="8dce5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dce5-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dce5-129">address</span><span class="sxs-lookup"><span data-stu-id="8dce5-129">address</span></span>|[<span data-ttu-id="8dce5-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="8dce5-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="8dce5-131">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-131">The street address of the business.</span></span>|
|<span data-ttu-id="8dce5-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="8dce5-132">businessHours</span></span>|<span data-ttu-id="8dce5-133">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="8dce5-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="8dce5-134">As horas de operação da empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="8dce5-135">businesstype</span><span class="sxs-lookup"><span data-stu-id="8dce5-135">businessType</span></span>|<span data-ttu-id="8dce5-136">String</span><span class="sxs-lookup"><span data-stu-id="8dce5-136">String</span></span>|<span data-ttu-id="8dce5-137">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="8dce5-137">The type of business.</span></span>|
|<span data-ttu-id="8dce5-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="8dce5-138">defaultCurrencyIso</span></span>|<span data-ttu-id="8dce5-139">String</span><span class="sxs-lookup"><span data-stu-id="8dce5-139">String</span></span>|<span data-ttu-id="8dce5-140">O código da moeda na qual a empresa opera em reservas da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8dce5-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="8dce5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8dce5-141">displayName</span></span>|<span data-ttu-id="8dce5-142">String</span><span class="sxs-lookup"><span data-stu-id="8dce5-142">String</span></span>|<span data-ttu-id="8dce5-143">Um nome para a empresa que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="8dce5-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="8dce5-144">email</span><span class="sxs-lookup"><span data-stu-id="8dce5-144">email</span></span>|<span data-ttu-id="8dce5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dce5-145">String</span></span>|<span data-ttu-id="8dce5-146">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-146">The email address for the business.</span></span>|
|<span data-ttu-id="8dce5-147">phone</span><span class="sxs-lookup"><span data-stu-id="8dce5-147">phone</span></span>|<span data-ttu-id="8dce5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dce5-148">String</span></span>|<span data-ttu-id="8dce5-149">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="8dce5-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="8dce5-150">schedulingPolicy</span></span>|[<span data-ttu-id="8dce5-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="8dce5-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="8dce5-152">Especifica como as reservas podem ser criadas para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="8dce5-153">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="8dce5-153">webSiteUrl</span></span>|<span data-ttu-id="8dce5-154">String</span><span class="sxs-lookup"><span data-stu-id="8dce5-154">String</span></span>|<span data-ttu-id="8dce5-155">A URL do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="8dce5-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="8dce5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dce5-156">Response</span></span>
<span data-ttu-id="8dce5-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dce5-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8dce5-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dce5-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dce5-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dce5-160">Request</span></span>
<span data-ttu-id="8dce5-161">O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão de negócios para uma hora e para a reserva antecipada até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="8dce5-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8dce5-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dce5-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8dce5-163">C#</span><span class="sxs-lookup"><span data-stu-id="8dce5-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dce5-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dce5-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dce5-165">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8dce5-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8dce5-166">Java</span><span class="sxs-lookup"><span data-stu-id="8dce5-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8dce5-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dce5-167">Response</span></span>
<span data-ttu-id="8dce5-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8dce5-168">The following is an example of the response.</span></span> <span data-ttu-id="8dce5-169">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8dce5-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8dce5-170">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dce5-170">All of the properties will be returned from an actual call.</span></span>
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
