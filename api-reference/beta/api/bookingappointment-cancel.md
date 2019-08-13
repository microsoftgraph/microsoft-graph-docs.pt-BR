---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ce8b34bd122b1a437dbc0069a2ab88c876fbf3ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318457"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="da725-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="da725-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da725-104">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="da725-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="da725-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da725-105">Permissions</span></span>
<span data-ttu-id="da725-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da725-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da725-108">Permission type</span></span>      | <span data-ttu-id="da725-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da725-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da725-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da725-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="da725-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="da725-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="da725-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da725-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da725-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da725-113">Not supported.</span></span>   |
|<span data-ttu-id="da725-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da725-114">Application</span></span> | <span data-ttu-id="da725-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da725-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="da725-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da725-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="da725-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da725-117">Request headers</span></span>
| <span data-ttu-id="da725-118">Nome</span><span class="sxs-lookup"><span data-stu-id="da725-118">Name</span></span>       | <span data-ttu-id="da725-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="da725-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da725-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="da725-120">Authorization</span></span>  | <span data-ttu-id="da725-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="da725-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="da725-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da725-122">Request body</span></span>
<span data-ttu-id="da725-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da725-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="da725-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="da725-124">Parameter</span></span>    | <span data-ttu-id="da725-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="da725-125">Type</span></span>   |<span data-ttu-id="da725-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="da725-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da725-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="da725-127">cancellationMessage</span></span>|<span data-ttu-id="da725-128">String</span><span class="sxs-lookup"><span data-stu-id="da725-128">String</span></span>|<span data-ttu-id="da725-129">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="da725-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="da725-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="da725-130">Response</span></span>
<span data-ttu-id="da725-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da725-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="da725-133">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="da725-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="da725-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da725-134">Example</span></span>
<span data-ttu-id="da725-135">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="da725-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da725-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da725-136">Request</span></span>
<span data-ttu-id="da725-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da725-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da725-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="da725-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="da725-139">C#</span><span class="sxs-lookup"><span data-stu-id="da725-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da725-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da725-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da725-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da725-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da725-142">Java</span><span class="sxs-lookup"><span data-stu-id="da725-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingappointment-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da725-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="da725-143">Response</span></span>
<span data-ttu-id="da725-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da725-144">The following is an example of the response.</span></span>
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
