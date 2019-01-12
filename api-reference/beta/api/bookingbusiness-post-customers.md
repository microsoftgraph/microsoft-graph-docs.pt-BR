---
title: Criar bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 555723fdb4eb7bacb2c876ed3fd87eb539a5239d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922253"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="f875e-104">Criar bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="f875e-104">Create bookingCustomer</span></span>

 > <span data-ttu-id="f875e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f875e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f875e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f875e-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f875e-107">Crie um novo objeto de [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="f875e-107">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f875e-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f875e-108">Permissions</span></span>
<span data-ttu-id="f875e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f875e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f875e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f875e-111">Permission type</span></span>      | <span data-ttu-id="f875e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f875e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f875e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f875e-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f875e-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f875e-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f875e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f875e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f875e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f875e-116">Not supported.</span></span>   |
|<span data-ttu-id="f875e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f875e-117">Application</span></span> | <span data-ttu-id="f875e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f875e-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f875e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f875e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="f875e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f875e-120">Request headers</span></span>
| <span data-ttu-id="f875e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f875e-121">Name</span></span>       | <span data-ttu-id="f875e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f875e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f875e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f875e-123">Authorization</span></span>  | <span data-ttu-id="f875e-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f875e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f875e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f875e-125">Request body</span></span>
<span data-ttu-id="f875e-126">No corpo da solicitação, fornece uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="f875e-126">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f875e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f875e-127">Response</span></span>
<span data-ttu-id="f875e-128">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingCustomer](../resources/bookingcustomer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f875e-128">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f875e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f875e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f875e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f875e-130">Request</span></span>
<span data-ttu-id="f875e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f875e-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="f875e-132">No corpo da solicitação, fornece uma representação JSON do objeto [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="f875e-132">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f875e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f875e-133">Response</span></span>
<span data-ttu-id="f875e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f875e-134">The following is an example of the response.</span></span> <span data-ttu-id="f875e-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f875e-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f875e-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f875e-136">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
