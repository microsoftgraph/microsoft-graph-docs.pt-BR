---
title: Obter bookingStaffMember
description: Obtenha as propriedades e os relacionamentos de um bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a45236dcd154b1e377a975bdd488a74b4433de94
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318093"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="b2bc2-103">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b2bc2-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2bc2-104">Obtenha as propriedades e os relacionamentos de um [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b2bc2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2bc2-105">Permissions</span></span>
<span data-ttu-id="b2bc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2bc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2bc2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2bc2-108">Permission type</span></span>      | <span data-ttu-id="b2bc2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2bc2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2bc2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2bc2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b2bc2-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="b2bc2-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b2bc2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2bc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2bc2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-113">Not supported.</span></span>   |
|<span data-ttu-id="b2bc2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2bc2-114">Application</span></span> | <span data-ttu-id="b2bc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b2bc2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2bc2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b2bc2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b2bc2-117">Optional query parameters</span></span>
<span data-ttu-id="b2bc2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2bc2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2bc2-119">Request headers</span></span>
| <span data-ttu-id="b2bc2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b2bc2-120">Name</span></span>      |<span data-ttu-id="b2bc2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2bc2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2bc2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2bc2-122">Authorization</span></span>  | <span data-ttu-id="b2bc2-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b2bc2-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2bc2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2bc2-124">Request body</span></span>
<span data-ttu-id="b2bc2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b2bc2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2bc2-126">Response</span></span>
<span data-ttu-id="b2bc2-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2bc2-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2bc2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2bc2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2bc2-129">Request</span></span>
<span data-ttu-id="b2bc2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2bc2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2bc2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2bc2-132">C#</span><span class="sxs-lookup"><span data-stu-id="b2bc2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2bc2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2bc2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2bc2-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b2bc2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b2bc2-135">Java</span><span class="sxs-lookup"><span data-stu-id="b2bc2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b2bc2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2bc2-136">Response</span></span>
<span data-ttu-id="b2bc2-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-137">The following is an example of the response.</span></span> <span data-ttu-id="b2bc2-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2bc2-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2bc2-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id": "71d64d0e-7225-49b6-b0b1-070d476cda51",
    "displayName": "Samantha Booth",
    "emailAddress": "samanthab@M365B489948.OnMicrosoft.com",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 0,
    "role": "administrator",
    "useBusinessHours": true,
    "workingHours": [
        {
            "day": "monday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "tuesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "wednesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "thursday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "friday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "saturday",
            "timeSlots": []
        },
        {
            "day": "sunday",
            "timeSlots": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
