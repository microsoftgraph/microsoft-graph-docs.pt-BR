---
title: Criar bookingBusiness
description: Crie uma nova empresa do Microsoft Bookings em um locatário.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 251d1b6d5e73b646216bdb152289808e93882d38
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047879"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="6fe81-103">Criar bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="6fe81-103">Create bookingBusiness</span></span>

<span data-ttu-id="6fe81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe81-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe81-105">Crie uma nova empresa do Microsoft Bookings em um locatário.</span><span class="sxs-lookup"><span data-stu-id="6fe81-105">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="6fe81-106">Esta é a primeira etapa na configuração de uma empresa do Bookings em que você deve especificar o nome de exibição comercial.</span><span class="sxs-lookup"><span data-stu-id="6fe81-106">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="6fe81-107">Você pode incluir outras informações, como endereço comercial, endereço do site e [](bookingbusiness-update.md) política de agendamento, ou definir essas informações posteriormente atualizando **o bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="6fe81-107">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fe81-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fe81-108">Permissions</span></span>
<span data-ttu-id="6fe81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fe81-111">Permission type</span></span>      | <span data-ttu-id="6fe81-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fe81-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fe81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fe81-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6fe81-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6fe81-114">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="6fe81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fe81-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fe81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fe81-116">Not supported.</span></span>   |
|<span data-ttu-id="6fe81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fe81-117">Application</span></span> | <span data-ttu-id="6fe81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fe81-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fe81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fe81-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="6fe81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe81-120">Request headers</span></span>
| <span data-ttu-id="6fe81-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6fe81-121">Name</span></span>       | <span data-ttu-id="6fe81-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fe81-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6fe81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe81-123">Authorization</span></span>  | <span data-ttu-id="6fe81-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6fe81-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe81-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe81-125">Request body</span></span>
<span data-ttu-id="6fe81-126">No corpo da solicitação, fornece uma representação JSON do [objeto bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="6fe81-126">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="6fe81-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe81-127">Response</span></span>
<span data-ttu-id="6fe81-128">Se tiver êxito, este método retornará `201, Created` o código de resposta e o objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe81-128">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe81-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fe81-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fe81-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fe81-130">Request</span></span>
<span data-ttu-id="6fe81-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fe81-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fe81-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fe81-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json

{
    "displayName":"Fourth Coffee",
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD"
}
```
# <a name="c"></a>[<span data-ttu-id="6fe81-133">C#</span><span class="sxs-lookup"><span data-stu-id="6fe81-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fe81-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fe81-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fe81-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fe81-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fe81-136">Java</span><span class="sxs-lookup"><span data-stu-id="6fe81-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingbusiness-from-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6fe81-137">No corpo da solicitação, fornece uma representação JSON do [objeto bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="6fe81-137">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6fe81-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fe81-138">Response</span></span>
<span data-ttu-id="6fe81-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fe81-139">The following is an example of the response.</span></span> <span data-ttu-id="6fe81-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6fe81-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"fourthcoffee@M365B489948.onmicrosoft.com",
    "displayName":"Fourth Coffee",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


