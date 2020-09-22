---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 42a12bfd05dddf6306f6de22b07b2029d2f39e2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988132"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="2342d-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="2342d-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="2342d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2342d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2342d-105">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="2342d-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2342d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2342d-106">Permissions</span></span>
<span data-ttu-id="2342d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2342d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2342d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2342d-109">Permission type</span></span>      | <span data-ttu-id="2342d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2342d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2342d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2342d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2342d-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="2342d-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2342d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2342d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2342d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2342d-114">Not supported.</span></span>   |
|<span data-ttu-id="2342d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2342d-115">Application</span></span> | <span data-ttu-id="2342d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2342d-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2342d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2342d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="2342d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2342d-118">Request headers</span></span>
| <span data-ttu-id="2342d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2342d-119">Name</span></span>       | <span data-ttu-id="2342d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2342d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2342d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2342d-121">Authorization</span></span>  | <span data-ttu-id="2342d-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2342d-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2342d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2342d-123">Request body</span></span>
<span data-ttu-id="2342d-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2342d-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2342d-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2342d-125">Parameter</span></span>    | <span data-ttu-id="2342d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2342d-126">Type</span></span>   |<span data-ttu-id="2342d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2342d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2342d-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="2342d-128">cancellationMessage</span></span>|<span data-ttu-id="2342d-129">String</span><span class="sxs-lookup"><span data-stu-id="2342d-129">String</span></span>|<span data-ttu-id="2342d-130">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="2342d-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="2342d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2342d-131">Response</span></span>
<span data-ttu-id="2342d-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2342d-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="2342d-134">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="2342d-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="2342d-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2342d-135">Example</span></span>
<span data-ttu-id="2342d-136">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2342d-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2342d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2342d-137">Request</span></span>
<span data-ttu-id="2342d-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2342d-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2342d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2342d-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2342d-140">C#</span><span class="sxs-lookup"><span data-stu-id="2342d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2342d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2342d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2342d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2342d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2342d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2342d-143">Response</span></span>
<span data-ttu-id="2342d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2342d-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


