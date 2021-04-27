---
title: Criar bookingCustomer
description: Crie um novo objeto bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5206c6969f2a0f9504cfecd347e7e215577caae1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047865"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="a3666-103">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="a3666-103">Create bookingCustomer</span></span>

<span data-ttu-id="a3666-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3666-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3666-105">Crie um novo [objeto bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="a3666-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3666-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3666-106">Permissions</span></span>
<span data-ttu-id="a3666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3666-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3666-109">Permission type</span></span>      | <span data-ttu-id="a3666-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3666-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3666-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3666-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a3666-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a3666-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a3666-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3666-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3666-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3666-114">Not supported.</span></span>   |
|<span data-ttu-id="a3666-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3666-115">Application</span></span> | <span data-ttu-id="a3666-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3666-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a3666-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3666-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="a3666-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3666-118">Request headers</span></span>
| <span data-ttu-id="a3666-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a3666-119">Name</span></span>       | <span data-ttu-id="a3666-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3666-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a3666-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3666-121">Authorization</span></span>  | <span data-ttu-id="a3666-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a3666-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3666-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3666-123">Request body</span></span>
<span data-ttu-id="a3666-124">No corpo da solicitação, fornece uma representação JSON do [objeto bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="a3666-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a3666-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3666-125">Response</span></span>
<span data-ttu-id="a3666-126">Se tiver êxito, este método retornará `201, Created` o código de resposta e o objeto [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3666-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3666-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3666-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3666-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3666-128">Request</span></span>
<span data-ttu-id="a3666-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3666-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3666-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3666-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
# <a name="c"></a>[<span data-ttu-id="a3666-131">C#</span><span class="sxs-lookup"><span data-stu-id="a3666-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3666-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3666-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3666-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3666-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3666-134">Java</span><span class="sxs-lookup"><span data-stu-id="a3666-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingcustomer-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a3666-135">No corpo da solicitação, fornece uma representação JSON do [objeto bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="a3666-135">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a3666-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3666-136">Response</span></span>
<span data-ttu-id="a3666-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3666-137">The following is an example of the response.</span></span> <span data-ttu-id="a3666-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3666-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


