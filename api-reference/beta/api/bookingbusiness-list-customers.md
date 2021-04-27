---
title: Listar clientes
description: Obter uma lista de objetos bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 9eff7f998ad5bf5f1c623e2a699c7c1be3636b8a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047900"
---
# <a name="list-customers"></a><span data-ttu-id="a4ad7-103">Listar clientes</span><span class="sxs-lookup"><span data-stu-id="a4ad7-103">List customers</span></span>

<span data-ttu-id="a4ad7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ad7-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ad7-105">Obter uma lista de [objetos bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-105">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4ad7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4ad7-106">Permissions</span></span>
<span data-ttu-id="a4ad7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ad7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4ad7-109">Permission type</span></span>      | <span data-ttu-id="a4ad7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4ad7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a4ad7-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a4ad7-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a4ad7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ad7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-114">Not supported.</span></span>   |
|<span data-ttu-id="a4ad7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4ad7-115">Application</span></span> | <span data-ttu-id="a4ad7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a4ad7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ad7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4ad7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4ad7-118">Optional query parameters</span></span>
<span data-ttu-id="a4ad7-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4ad7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ad7-120">Request headers</span></span>
| <span data-ttu-id="a4ad7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a4ad7-121">Name</span></span>      |<span data-ttu-id="a4ad7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4ad7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a4ad7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ad7-123">Authorization</span></span>  | <span data-ttu-id="a4ad7-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a4ad7-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ad7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ad7-125">Request body</span></span>
<span data-ttu-id="a4ad7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a4ad7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ad7-127">Response</span></span>
<span data-ttu-id="a4ad7-128">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-128">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4ad7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4ad7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4ad7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4ad7-130">Request</span></span>
<span data-ttu-id="a4ad7-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4ad7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ad7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="c"></a>[<span data-ttu-id="a4ad7-133">C#</span><span class="sxs-lookup"><span data-stu-id="a4ad7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4ad7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ad7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4ad7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4ad7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4ad7-136">Java</span><span class="sxs-lookup"><span data-stu-id="a4ad7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-customers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a4ad7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4ad7-137">Response</span></span>
<span data-ttu-id="a4ad7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-138">The following is an example of the response.</span></span> <span data-ttu-id="a4ad7-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
