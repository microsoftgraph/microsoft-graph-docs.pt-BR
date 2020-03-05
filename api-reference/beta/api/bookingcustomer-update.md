---
title: Atualizar bookingcustomer
description: Atualiza as propriedades de um objeto bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c1af0dc924c923b9a9c0c2fa6093120ccbfa3cf7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441106"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="cad99-103">Atualizar bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="cad99-103">Update bookingcustomer</span></span>

<span data-ttu-id="cad99-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cad99-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cad99-105">Atualiza as propriedades de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="cad99-105">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cad99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cad99-106">Permissions</span></span>
<span data-ttu-id="cad99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cad99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cad99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cad99-109">Permission type</span></span>      | <span data-ttu-id="cad99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cad99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cad99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cad99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cad99-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="cad99-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cad99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cad99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cad99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cad99-114">Not supported.</span></span>   |
|<span data-ttu-id="cad99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cad99-115">Application</span></span> | <span data-ttu-id="cad99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cad99-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cad99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cad99-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cad99-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="cad99-118">Optional request headers</span></span>
| <span data-ttu-id="cad99-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cad99-119">Name</span></span>       | <span data-ttu-id="cad99-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad99-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cad99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cad99-121">Authorization</span></span>  | <span data-ttu-id="cad99-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cad99-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cad99-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cad99-123">Request body</span></span>
<span data-ttu-id="cad99-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cad99-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cad99-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cad99-127">Property</span></span>     | <span data-ttu-id="cad99-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cad99-128">Type</span></span>   |<span data-ttu-id="cad99-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cad99-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cad99-130">displayName</span><span class="sxs-lookup"><span data-stu-id="cad99-130">displayName</span></span>|<span data-ttu-id="cad99-131">String</span><span class="sxs-lookup"><span data-stu-id="cad99-131">String</span></span>|<span data-ttu-id="cad99-132">O nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="cad99-132">The name of the customer.</span></span>|
|<span data-ttu-id="cad99-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cad99-133">emailAddress</span></span>|<span data-ttu-id="cad99-134">String</span><span class="sxs-lookup"><span data-stu-id="cad99-134">String</span></span>|<span data-ttu-id="cad99-135">O endereço SMTP do cliente.</span><span class="sxs-lookup"><span data-stu-id="cad99-135">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="cad99-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad99-136">Response</span></span>
<span data-ttu-id="cad99-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingCustomer](../resources/bookingcustomer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cad99-137">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cad99-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cad99-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cad99-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cad99-139">Request</span></span>
<span data-ttu-id="cad99-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cad99-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cad99-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cad99-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
# <a name="c"></a>[<span data-ttu-id="cad99-142">C#</span><span class="sxs-lookup"><span data-stu-id="cad99-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cad99-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cad99-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cad99-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cad99-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cad99-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cad99-145">Response</span></span>
<span data-ttu-id="cad99-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cad99-146">The following is an example of the response.</span></span> <span data-ttu-id="cad99-147">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cad99-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cad99-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cad99-148">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
