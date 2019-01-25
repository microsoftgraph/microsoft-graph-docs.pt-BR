---
title: Criar bookingBusiness
description: Crie um novo negócio Microsoft Bookings em um locatário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a9217392953d287689dca7a7b6f4c74fbe6383
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519245"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="3d1a4-103">Criar bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="3d1a4-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d1a4-104">Crie um novo negócio Microsoft Bookings em um locatário.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="3d1a4-105">Esta é a primeira etapa na configuração de uma empresa reservas onde você deve especificar o nome de exibição de negócios.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="3d1a4-106">Você pode incluir outras informações como endereço comercial, o endereço do site e a diretiva de agendamento, ou definir essas informações posteriormente através da [atualização](bookingbusiness-update.md) , o **bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d1a4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d1a4-107">Permissions</span></span>
<span data-ttu-id="3d1a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d1a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d1a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d1a4-110">Permission type</span></span>      | <span data-ttu-id="3d1a4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d1a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d1a4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d1a4-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3d1a4-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3d1a4-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="3d1a4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d1a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d1a4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-115">Not supported.</span></span>   |
|<span data-ttu-id="3d1a4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d1a4-116">Application</span></span> | <span data-ttu-id="3d1a4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d1a4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d1a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="3d1a4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d1a4-119">Request headers</span></span>
| <span data-ttu-id="3d1a4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3d1a4-120">Name</span></span>       | <span data-ttu-id="3d1a4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d1a4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3d1a4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d1a4-122">Authorization</span></span>  | <span data-ttu-id="3d1a4-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3d1a4-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d1a4-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d1a4-124">Request body</span></span>
<span data-ttu-id="3d1a4-125">No corpo da solicitação, fornece uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="3d1a4-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="3d1a4-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d1a4-126">Response</span></span>
<span data-ttu-id="3d1a4-127">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d1a4-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d1a4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d1a4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d1a4-129">Request</span></span>
<span data-ttu-id="3d1a4-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="3d1a4-131">No corpo da solicitação, fornece uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="3d1a4-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3d1a4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d1a4-132">Response</span></span>
<span data-ttu-id="3d1a4-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-133">The following is an example of the response.</span></span> <span data-ttu-id="3d1a4-134">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3d1a4-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d1a4-135">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
