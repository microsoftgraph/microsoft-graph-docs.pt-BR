---
title: Obter bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 38a0fa87bc3b81c493914b14a8c35a01dad11689
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27989988"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="6f6fa-104">Obter bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="6f6fa-104">Get bookingCustomer</span></span>

 > <span data-ttu-id="6f6fa-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f6fa-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="6f6fa-107">Obtenha as propriedades e relacionamentos de um objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="6f6fa-107">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f6fa-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="6f6fa-108">Permissions</span></span>
<span data-ttu-id="6f6fa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6fa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f6fa-111">Permission type</span></span>      | <span data-ttu-id="6f6fa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f6fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6fa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f6fa-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f6fa-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6f6fa-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6f6fa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f6fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-116">Not supported.</span></span>   |
|<span data-ttu-id="6f6fa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6fa-117">Application</span></span> | <span data-ttu-id="6f6fa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="6f6fa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f6fa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f6fa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f6fa-120">Optional query parameters</span></span>
<span data-ttu-id="6f6fa-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f6fa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6fa-122">Request headers</span></span>
| <span data-ttu-id="6f6fa-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6f6fa-123">Name</span></span>      |<span data-ttu-id="6f6fa-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f6fa-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f6fa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f6fa-125">Authorization</span></span>  | <span data-ttu-id="6f6fa-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6f6fa-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6fa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6fa-127">Request body</span></span>
<span data-ttu-id="6f6fa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6f6fa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6fa-129">Response</span></span>
<span data-ttu-id="6f6fa-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-130">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6f6fa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f6fa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f6fa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6fa-132">Request</span></span>
<span data-ttu-id="6f6fa-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="6f6fa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6fa-134">Response</span></span>
<span data-ttu-id="6f6fa-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-135">The following is an example of the response.</span></span> <span data-ttu-id="6f6fa-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6f6fa-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f6fa-137">All of the properties will be returned from an actual call.</span></span>
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
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
