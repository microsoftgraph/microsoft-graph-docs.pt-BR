---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 91c9da27446d7588c806f3262b5060780071a78d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441316"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="aef19-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="aef19-103">bookingAppointment: cancel</span></span>

<span data-ttu-id="aef19-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aef19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aef19-105">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="aef19-105">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="aef19-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aef19-106">Permissions</span></span>
<span data-ttu-id="aef19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aef19-109">Permission type</span></span>      | <span data-ttu-id="aef19-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aef19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aef19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aef19-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aef19-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="aef19-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="aef19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aef19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aef19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef19-114">Not supported.</span></span>   |
|<span data-ttu-id="aef19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aef19-115">Application</span></span> | <span data-ttu-id="aef19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef19-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="aef19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aef19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="aef19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aef19-118">Request headers</span></span>
| <span data-ttu-id="aef19-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aef19-119">Name</span></span>       | <span data-ttu-id="aef19-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aef19-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aef19-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aef19-121">Authorization</span></span>  | <span data-ttu-id="aef19-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="aef19-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aef19-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aef19-123">Request body</span></span>
<span data-ttu-id="aef19-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef19-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aef19-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aef19-125">Parameter</span></span>    | <span data-ttu-id="aef19-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="aef19-126">Type</span></span>   |<span data-ttu-id="aef19-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="aef19-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aef19-128">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="aef19-128">cancellationMessage</span></span>|<span data-ttu-id="aef19-129">String</span><span class="sxs-lookup"><span data-stu-id="aef19-129">String</span></span>|<span data-ttu-id="aef19-130">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="aef19-130">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="aef19-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef19-131">Response</span></span>
<span data-ttu-id="aef19-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aef19-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="aef19-134">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="aef19-134">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="aef19-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aef19-135">Example</span></span>
<span data-ttu-id="aef19-136">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aef19-136">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aef19-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aef19-137">Request</span></span>
<span data-ttu-id="aef19-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef19-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aef19-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="aef19-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="aef19-140">C#</span><span class="sxs-lookup"><span data-stu-id="aef19-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aef19-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aef19-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aef19-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aef19-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aef19-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef19-143">Response</span></span>
<span data-ttu-id="aef19-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aef19-144">The following is an example of the response.</span></span>
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
