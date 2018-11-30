---
title: Clientes de lista
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: a46e8dcc39b69e8391829c176eb01d075d23fccf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035024"
---
# <a name="list-customers"></a><span data-ttu-id="05054-104">Clientes de lista</span><span class="sxs-lookup"><span data-stu-id="05054-104">List customers</span></span>

 > <span data-ttu-id="05054-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="05054-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05054-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05054-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="05054-107">Obtenha uma lista de objetos [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="05054-107">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="05054-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="05054-108">Permissions</span></span>
<span data-ttu-id="05054-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05054-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05054-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05054-111">Permission type</span></span>      | <span data-ttu-id="05054-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05054-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05054-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05054-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="05054-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="05054-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="05054-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05054-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05054-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05054-116">Not supported.</span></span>   |
|<span data-ttu-id="05054-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05054-117">Application</span></span> | <span data-ttu-id="05054-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05054-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="05054-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05054-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05054-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05054-120">Optional query parameters</span></span>
<span data-ttu-id="05054-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05054-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05054-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05054-122">Request headers</span></span>
| <span data-ttu-id="05054-123">Nome</span><span class="sxs-lookup"><span data-stu-id="05054-123">Name</span></span>      |<span data-ttu-id="05054-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="05054-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05054-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="05054-125">Authorization</span></span>  | <span data-ttu-id="05054-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="05054-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="05054-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05054-127">Request body</span></span>
<span data-ttu-id="05054-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05054-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="05054-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="05054-129">Response</span></span>
<span data-ttu-id="05054-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05054-130">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05054-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05054-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05054-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05054-132">Request</span></span>
<span data-ttu-id="05054-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05054-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="05054-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="05054-134">Response</span></span>
<span data-ttu-id="05054-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05054-135">The following is an example of the response.</span></span> <span data-ttu-id="05054-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="05054-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="05054-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05054-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->