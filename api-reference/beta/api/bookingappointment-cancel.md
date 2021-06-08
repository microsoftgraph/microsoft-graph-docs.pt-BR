---
title: 'bookingAppointment: cancel'
description: Cancele o bookingAppointment especificado no bookingbusiness especificado e envie uma mensagem aos clientes envolvidos e aos membros da equipe.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4d05157faf95beaf6dab95742314472586f00063
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786268"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="0c7a9-103">bookingAppointment: cancel</span><span class="sxs-lookup"><span data-stu-id="0c7a9-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="0c7a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c7a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c7a9-105">Cancele o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e envie uma mensagem aos clientes envolvidos e aos membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c7a9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0c7a9-106">Permissions</span></span>
<span data-ttu-id="0c7a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c7a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c7a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c7a9-109">Permission type</span></span>      | <span data-ttu-id="0c7a9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c7a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c7a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c7a9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c7a9-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0c7a9-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0c7a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c7a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c7a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-114">Not supported.</span></span>   |
|<span data-ttu-id="0c7a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c7a9-115">Application</span></span> | <span data-ttu-id="0c7a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0c7a9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7a9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="0c7a9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7a9-118">Request headers</span></span>
| <span data-ttu-id="0c7a9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0c7a9-119">Name</span></span>       | <span data-ttu-id="0c7a9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7a9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0c7a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c7a9-121">Authorization</span></span>  | <span data-ttu-id="0c7a9-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0c7a9-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c7a9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7a9-123">Request body</span></span>
<span data-ttu-id="0c7a9-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c7a9-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0c7a9-125">Parameter</span></span>    | <span data-ttu-id="0c7a9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c7a9-126">Type</span></span>   |<span data-ttu-id="0c7a9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7a9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c7a9-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="0c7a9-128">cancellationMessage</span></span>|<span data-ttu-id="0c7a9-129">String</span><span class="sxs-lookup"><span data-stu-id="0c7a9-129">String</span></span>|<span data-ttu-id="0c7a9-130">Uma mensagem para confirmar com o cliente que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="0c7a9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7a9-131">Response</span></span>
<span data-ttu-id="0c7a9-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="0c7a9-134">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="0c7a9-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="0c7a9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c7a9-135">Example</span></span>
<span data-ttu-id="0c7a9-136">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c7a9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c7a9-137">Request</span></span>
<span data-ttu-id="0c7a9-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c7a9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c7a9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```
# <a name="c"></a>[<span data-ttu-id="0c7a9-140">C#</span><span class="sxs-lookup"><span data-stu-id="0c7a9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c7a9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c7a9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c7a9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c7a9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0c7a9-143">Java</span><span class="sxs-lookup"><span data-stu-id="0c7a9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0c7a9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c7a9-144">Response</span></span>
<span data-ttu-id="0c7a9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0c7a9-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


