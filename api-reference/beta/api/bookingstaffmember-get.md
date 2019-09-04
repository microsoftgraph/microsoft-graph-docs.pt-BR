---
title: Obter bookingStaffMember
description: Obtenha as propriedades e os relacionamentos de um bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 218017ced4927f651e1ad370ab6b34360951c25c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718811"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="faaf9-103">Obter bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="faaf9-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faaf9-104">Obtenha as propriedades e os relacionamentos de um [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="faaf9-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="faaf9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="faaf9-105">Permissions</span></span>
<span data-ttu-id="faaf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faaf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faaf9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faaf9-108">Permission type</span></span>      | <span data-ttu-id="faaf9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="faaf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faaf9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faaf9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="faaf9-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="faaf9-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="faaf9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faaf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faaf9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faaf9-113">Not supported.</span></span>   |
|<span data-ttu-id="faaf9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faaf9-114">Application</span></span> | <span data-ttu-id="faaf9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faaf9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="faaf9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faaf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="faaf9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="faaf9-117">Optional query parameters</span></span>
<span data-ttu-id="faaf9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="faaf9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="faaf9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faaf9-119">Request headers</span></span>
| <span data-ttu-id="faaf9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="faaf9-120">Name</span></span>      |<span data-ttu-id="faaf9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="faaf9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="faaf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="faaf9-122">Authorization</span></span>  | <span data-ttu-id="faaf9-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="faaf9-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="faaf9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faaf9-124">Request body</span></span>
<span data-ttu-id="faaf9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="faaf9-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="faaf9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="faaf9-126">Response</span></span>
<span data-ttu-id="faaf9-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="faaf9-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="faaf9-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faaf9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="faaf9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faaf9-129">Request</span></span>
<span data-ttu-id="faaf9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="faaf9-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="faaf9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="faaf9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="faaf9-132">C#</span><span class="sxs-lookup"><span data-stu-id="faaf9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="faaf9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="faaf9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="faaf9-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="faaf9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="faaf9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="faaf9-135">Response</span></span>
<span data-ttu-id="faaf9-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="faaf9-136">The following is an example of the response.</span></span> <span data-ttu-id="faaf9-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="faaf9-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="faaf9-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="faaf9-138">All of the properties will be returned from an actual call.</span></span>
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
