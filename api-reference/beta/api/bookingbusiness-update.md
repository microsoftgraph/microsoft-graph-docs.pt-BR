---
title: Atualizar bookingbusiness
description: Atualiza as propriedades de um objeto bookingBusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b820d65a50b2a07bd1c3e95936bc6ee304f20d96
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376601"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="d8d59-103">Atualizar bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="d8d59-103">Update bookingbusiness</span></span>

<span data-ttu-id="d8d59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8d59-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8d59-105">Atualiza as propriedades de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="d8d59-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d8d59-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8d59-106">Permissions</span></span>
<span data-ttu-id="d8d59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8d59-109">Permission type</span></span>      | <span data-ttu-id="d8d59-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8d59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8d59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8d59-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d8d59-112">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d8d59-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d8d59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8d59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8d59-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d59-114">Not supported.</span></span>   |
|<span data-ttu-id="d8d59-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8d59-115">Application</span></span> | <span data-ttu-id="d8d59-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d59-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d8d59-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d8d59-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d8d59-118">Optional request headers</span></span>
| <span data-ttu-id="d8d59-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d8d59-119">Name</span></span>       | <span data-ttu-id="d8d59-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d59-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d8d59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8d59-121">Authorization</span></span>  | <span data-ttu-id="d8d59-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d8d59-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d59-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d59-123">Request body</span></span>
<span data-ttu-id="d8d59-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d8d59-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d8d59-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d59-127">Property</span></span>     | <span data-ttu-id="d8d59-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d59-128">Type</span></span>   |<span data-ttu-id="d8d59-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d59-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8d59-130">address</span><span class="sxs-lookup"><span data-stu-id="d8d59-130">address</span></span>|[<span data-ttu-id="d8d59-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d8d59-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="d8d59-132">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-132">The street address of the business.</span></span>|
|<span data-ttu-id="d8d59-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="d8d59-133">businessHours</span></span>|<span data-ttu-id="d8d59-134">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="d8d59-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="d8d59-135">As horas de operação da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="d8d59-136">businesstype</span><span class="sxs-lookup"><span data-stu-id="d8d59-136">businessType</span></span>|<span data-ttu-id="d8d59-137">String</span><span class="sxs-lookup"><span data-stu-id="d8d59-137">String</span></span>|<span data-ttu-id="d8d59-138">O tipo de negócio.</span><span class="sxs-lookup"><span data-stu-id="d8d59-138">The type of business.</span></span>|
|<span data-ttu-id="d8d59-139">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="d8d59-139">defaultCurrencyIso</span></span>|<span data-ttu-id="d8d59-140">String</span><span class="sxs-lookup"><span data-stu-id="d8d59-140">String</span></span>|<span data-ttu-id="d8d59-141">O código da moeda na qual a empresa opera em reservas da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d8d59-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="d8d59-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d8d59-142">displayName</span></span>|<span data-ttu-id="d8d59-143">String</span><span class="sxs-lookup"><span data-stu-id="d8d59-143">String</span></span>|<span data-ttu-id="d8d59-144">Um nome para a empresa que faz interface com clientes.</span><span class="sxs-lookup"><span data-stu-id="d8d59-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="d8d59-145">email</span><span class="sxs-lookup"><span data-stu-id="d8d59-145">email</span></span>|<span data-ttu-id="d8d59-146">String</span><span class="sxs-lookup"><span data-stu-id="d8d59-146">String</span></span>|<span data-ttu-id="d8d59-147">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-147">The email address for the business.</span></span>|
|<span data-ttu-id="d8d59-148">phone</span><span class="sxs-lookup"><span data-stu-id="d8d59-148">phone</span></span>|<span data-ttu-id="d8d59-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8d59-149">String</span></span>|<span data-ttu-id="d8d59-150">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="d8d59-151">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d8d59-151">schedulingPolicy</span></span>|[<span data-ttu-id="d8d59-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="d8d59-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="d8d59-153">Especifica como as reservas podem ser criadas para essa empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="d8d59-154">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="d8d59-154">webSiteUrl</span></span>|<span data-ttu-id="d8d59-155">String</span><span class="sxs-lookup"><span data-stu-id="d8d59-155">String</span></span>|<span data-ttu-id="d8d59-156">A URL do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="d8d59-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="d8d59-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d59-157">Response</span></span>
<span data-ttu-id="d8d59-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d59-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8d59-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8d59-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8d59-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d59-161">Request</span></span>
<span data-ttu-id="d8d59-162">O exemplo a seguir atualiza o endereço de email comercial e a política de agendamento, para alterar o intervalo de tempo de reserva padrão de negócios para uma hora e para a reserva antecipada até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="d8d59-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8d59-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d59-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8d59-164">C#</span><span class="sxs-lookup"><span data-stu-id="d8d59-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8d59-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8d59-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8d59-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8d59-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8d59-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d59-167">Response</span></span>
<span data-ttu-id="d8d59-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d59-168">The following is an example of the response.</span></span> <span data-ttu-id="d8d59-169">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d8d59-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d8d59-170">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8d59-170">All of the properties will be returned from an actual call.</span></span>
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
