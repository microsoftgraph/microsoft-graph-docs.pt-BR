---
title: Lista bookingCurrencies
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 146fc1197a8ef206e78304d81c30878a67eeafad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033091"
---
# <a name="list-bookingcurrencies"></a><span data-ttu-id="bd7fc-104">Lista bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="bd7fc-104">List bookingCurrencies</span></span>

 > <span data-ttu-id="bd7fc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd7fc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="bd7fc-107">Obtenha uma lista de objetos de [bookingCurrency](../resources/bookingcurrency.md) disponíveis para uma empresa Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-107">Get a list of [bookingCurrency](../resources/bookingcurrency.md) objects available to a Microsoft Bookings business.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd7fc-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bd7fc-108">Permissions</span></span>
<span data-ttu-id="bd7fc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd7fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd7fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd7fc-111">Permission type</span></span>      | <span data-ttu-id="bd7fc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd7fc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd7fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd7fc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bd7fc-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bd7fc-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bd7fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd7fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd7fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-116">Not supported.</span></span>   |
|<span data-ttu-id="bd7fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd7fc-117">Application</span></span> | <span data-ttu-id="bd7fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="bd7fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd7fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd7fc-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd7fc-120">Optional query parameters</span></span>
<span data-ttu-id="bd7fc-121">Este método oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta, incluindo $count, $filter, $select, $skip, Skip e $top.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response, including $count, $filter, $select, $skip, and $top.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd7fc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7fc-122">Request headers</span></span>
| <span data-ttu-id="bd7fc-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bd7fc-123">Name</span></span>      |<span data-ttu-id="bd7fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd7fc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd7fc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd7fc-125">Authorization</span></span>  | <span data-ttu-id="bd7fc-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bd7fc-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd7fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7fc-127">Request body</span></span>
<span data-ttu-id="bd7fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bd7fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd7fc-129">Response</span></span>
<span data-ttu-id="bd7fc-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-130">If successful, this method returns a `200 OK` response code and collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd7fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd7fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd7fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd7fc-132">Request</span></span>
<span data-ttu-id="bd7fc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrencies"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies
```
##### <a name="response"></a><span data-ttu-id="bd7fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd7fc-134">Response</span></span>
<span data-ttu-id="bd7fc-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-135">The following is an example of the response.</span></span> <span data-ttu-id="bd7fc-136">Observação: No objeto response mostrado aqui é truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-136">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="bd7fc-137">Serão retornados todos os moedas com suporte e as propriedades de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd7fc-137">All of the supported currencies and properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingCurrencies",
    "value":[
        {
            "id":"AED",
            "symbol":"د.إ.‏"
        },
        {
            "id":"AFN",
            "symbol":"؋"
        },
        {
            "id":"ALL",
            "symbol":"Lekë"
        },
        {
            "id":"AMD",
            "symbol":"֏"
        },
        {
            "id":"USD",
            "symbol":"$"
        },
        {
            "id":"YER",
            "symbol":"ر.ي.‏"
        },
        {
            "id":"ZAR",
            "symbol":"R"
        },
        {
            "id":"ZMW",
            "symbol":"K"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List bookingCurrencies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->