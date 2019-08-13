---
title: Criar bookingBusiness
description: Criar uma nova empresa de livros da Microsoft em um locatário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5b167b0e3ffe6697ff74cf11f477f01a3b28a0d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318275"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="20dd0-103">Criar bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="20dd0-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20dd0-104">Criar uma nova empresa de livros da Microsoft em um locatário.</span><span class="sxs-lookup"><span data-stu-id="20dd0-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="20dd0-105">Esta é a primeira etapa para configurar uma empresa de reservas onde você deve especificar o nome de exibição comercial.</span><span class="sxs-lookup"><span data-stu-id="20dd0-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="20dd0-106">Você pode incluir outras informações, como endereço comercial, endereço do site da Web e política de agendamento, ou definir essas informações [](bookingbusiness-update.md) mais tarde, atualizando o **bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="20dd0-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="20dd0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20dd0-107">Permissions</span></span>
<span data-ttu-id="20dd0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20dd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20dd0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20dd0-110">Permission type</span></span>      | <span data-ttu-id="20dd0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20dd0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20dd0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20dd0-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="20dd0-113">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="20dd0-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="20dd0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20dd0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20dd0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20dd0-115">Not supported.</span></span>   |
|<span data-ttu-id="20dd0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20dd0-116">Application</span></span> | <span data-ttu-id="20dd0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20dd0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20dd0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20dd0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="20dd0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20dd0-119">Request headers</span></span>
| <span data-ttu-id="20dd0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="20dd0-120">Name</span></span>       | <span data-ttu-id="20dd0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="20dd0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20dd0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20dd0-122">Authorization</span></span>  | <span data-ttu-id="20dd0-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="20dd0-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="20dd0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20dd0-124">Request body</span></span>
<span data-ttu-id="20dd0-125">No corpo da solicitação, forneça uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="20dd0-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="20dd0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="20dd0-126">Response</span></span>
<span data-ttu-id="20dd0-127">Se bem-sucedido, este método retorna `201, Created` o código de resposta e o objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20dd0-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20dd0-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20dd0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20dd0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20dd0-129">Request</span></span>
<span data-ttu-id="20dd0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="20dd0-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20dd0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="20dd0-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="20dd0-132">C#</span><span class="sxs-lookup"><span data-stu-id="20dd0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20dd0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20dd0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20dd0-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="20dd0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="20dd0-135">Java</span><span class="sxs-lookup"><span data-stu-id="20dd0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingbusiness-from-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="20dd0-136">No corpo da solicitação, forneça uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="20dd0-136">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="20dd0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="20dd0-137">Response</span></span>
<span data-ttu-id="20dd0-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20dd0-138">The following is an example of the response.</span></span> <span data-ttu-id="20dd0-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="20dd0-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="20dd0-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20dd0-140">All of the properties will be returned from an actual call.</span></span>
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
