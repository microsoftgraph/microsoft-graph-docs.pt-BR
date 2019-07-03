---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3673b1b97341ce679e37478d21f1afa6e582048e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439382"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="60c32-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="60c32-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60c32-104">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="60c32-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="60c32-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="60c32-105">Permissions</span></span>
<span data-ttu-id="60c32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60c32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60c32-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60c32-108">Permission type</span></span>      | <span data-ttu-id="60c32-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60c32-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60c32-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60c32-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="60c32-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="60c32-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="60c32-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60c32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60c32-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60c32-113">Not supported.</span></span>   |
|<span data-ttu-id="60c32-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60c32-114">Application</span></span> | <span data-ttu-id="60c32-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60c32-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="60c32-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60c32-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="60c32-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60c32-117">Request headers</span></span>
| <span data-ttu-id="60c32-118">Nome</span><span class="sxs-lookup"><span data-stu-id="60c32-118">Name</span></span>       | <span data-ttu-id="60c32-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c32-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60c32-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="60c32-120">Authorization</span></span>  | <span data-ttu-id="60c32-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="60c32-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="60c32-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60c32-122">Request body</span></span>
<span data-ttu-id="60c32-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60c32-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60c32-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="60c32-124">Parameter</span></span>    | <span data-ttu-id="60c32-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="60c32-125">Type</span></span>   |<span data-ttu-id="60c32-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c32-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60c32-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="60c32-127">cancellationMessage</span></span>|<span data-ttu-id="60c32-128">String</span><span class="sxs-lookup"><span data-stu-id="60c32-128">String</span></span>|<span data-ttu-id="60c32-129">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="60c32-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="60c32-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60c32-130">Response</span></span>
<span data-ttu-id="60c32-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60c32-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="60c32-133">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="60c32-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="60c32-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60c32-134">Example</span></span>
<span data-ttu-id="60c32-135">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="60c32-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60c32-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60c32-136">Request</span></span>
<span data-ttu-id="60c32-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60c32-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60c32-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="60c32-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="60c32-139">C#</span><span class="sxs-lookup"><span data-stu-id="60c32-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingappointment-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60c32-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="60c32-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingappointment-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60c32-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="60c32-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingappointment-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="60c32-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="60c32-142">Response</span></span>
<span data-ttu-id="60c32-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60c32-143">The following is an example of the response.</span></span>
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
