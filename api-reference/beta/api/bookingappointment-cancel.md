---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d2ef29421b5d79f30d8657a1caf05f5fae1e3890
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258233"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="f6529-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="f6529-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6529-104">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="f6529-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6529-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6529-105">Permissions</span></span>
<span data-ttu-id="f6529-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6529-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6529-108">Permission type</span></span>      | <span data-ttu-id="f6529-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6529-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6529-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6529-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f6529-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="f6529-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f6529-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6529-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6529-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6529-113">Not supported.</span></span>   |
|<span data-ttu-id="f6529-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6529-114">Application</span></span> | <span data-ttu-id="f6529-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6529-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f6529-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6529-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="f6529-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6529-117">Request headers</span></span>
| <span data-ttu-id="f6529-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f6529-118">Name</span></span>       | <span data-ttu-id="f6529-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6529-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6529-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6529-120">Authorization</span></span>  | <span data-ttu-id="f6529-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f6529-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6529-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6529-122">Request body</span></span>
<span data-ttu-id="f6529-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6529-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6529-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f6529-124">Parameter</span></span>    | <span data-ttu-id="f6529-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6529-125">Type</span></span>   |<span data-ttu-id="f6529-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6529-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6529-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="f6529-127">cancellationMessage</span></span>|<span data-ttu-id="f6529-128">String</span><span class="sxs-lookup"><span data-stu-id="f6529-128">String</span></span>|<span data-ttu-id="f6529-129">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="f6529-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="f6529-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6529-130">Response</span></span>
<span data-ttu-id="f6529-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6529-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f6529-133">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="f6529-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="f6529-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f6529-134">Example</span></span>
<span data-ttu-id="f6529-135">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f6529-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f6529-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6529-136">Request</span></span>
<span data-ttu-id="f6529-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6529-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f6529-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6529-138">Response</span></span>
<span data-ttu-id="f6529-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6529-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f6529-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="f6529-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f6529-141">C#</span><span class="sxs-lookup"><span data-stu-id="f6529-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6529-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6529-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f6529-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f6529-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
