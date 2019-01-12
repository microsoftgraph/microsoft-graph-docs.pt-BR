---
title: Criar bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: aa5c4b9eaa2426736d23f42856d19ab14e6a1a43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922316"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="0ce56-104">Criar bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="0ce56-104">Create bookingBusiness</span></span>

 > <span data-ttu-id="0ce56-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ce56-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ce56-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ce56-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="0ce56-107">Crie um novo negócio Microsoft Bookings em um locatário.</span><span class="sxs-lookup"><span data-stu-id="0ce56-107">Create a new Microsoft Bookings business in a tenant.</span></span> 

<span data-ttu-id="0ce56-108">Esta é a primeira etapa na configuração de uma empresa reservas onde você deve especificar o nome de exibição de negócios.</span><span class="sxs-lookup"><span data-stu-id="0ce56-108">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="0ce56-109">Você pode incluir outras informações como endereço comercial, o endereço do site e a diretiva de agendamento, ou definir essas informações posteriormente através da [atualização](bookingbusiness-update.md) , o **bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="0ce56-109">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ce56-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ce56-110">Permissions</span></span>
<span data-ttu-id="0ce56-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ce56-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ce56-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ce56-113">Permission type</span></span>      | <span data-ttu-id="0ce56-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ce56-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce56-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ce56-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ce56-116">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0ce56-116">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="0ce56-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ce56-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce56-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce56-118">Not supported.</span></span>   |
|<span data-ttu-id="0ce56-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ce56-119">Application</span></span> | <span data-ttu-id="0ce56-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce56-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0ce56-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce56-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="0ce56-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce56-122">Request headers</span></span>
| <span data-ttu-id="0ce56-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0ce56-123">Name</span></span>       | <span data-ttu-id="0ce56-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce56-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ce56-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ce56-125">Authorization</span></span>  | <span data-ttu-id="0ce56-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0ce56-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce56-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce56-127">Request body</span></span>
<span data-ttu-id="0ce56-128">No corpo da solicitação, fornece uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="0ce56-128">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0ce56-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ce56-129">Response</span></span>
<span data-ttu-id="0ce56-130">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ce56-130">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ce56-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ce56-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ce56-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce56-132">Request</span></span>
<span data-ttu-id="0ce56-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ce56-133">The following is an example of the request.</span></span>
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
<span data-ttu-id="0ce56-134">No corpo da solicitação, fornece uma representação JSON do objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="0ce56-134">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0ce56-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ce56-135">Response</span></span>
<span data-ttu-id="0ce56-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ce56-136">The following is an example of the response.</span></span> <span data-ttu-id="0ce56-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0ce56-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0ce56-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ce56-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
