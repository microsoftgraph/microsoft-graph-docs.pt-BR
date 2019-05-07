---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c96ed0403e59f4b2dd357514168361fc3bc683f6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636531"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="52de8-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="52de8-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52de8-104">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="52de8-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="52de8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52de8-105">Permissions</span></span>
<span data-ttu-id="52de8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52de8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52de8-108">Permission type</span></span>      | <span data-ttu-id="52de8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52de8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52de8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52de8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="52de8-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="52de8-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="52de8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52de8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52de8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52de8-113">Not supported.</span></span>   |
|<span data-ttu-id="52de8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52de8-114">Application</span></span> | <span data-ttu-id="52de8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52de8-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="52de8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52de8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="52de8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52de8-117">Request headers</span></span>
| <span data-ttu-id="52de8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52de8-118">Name</span></span>       | <span data-ttu-id="52de8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52de8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="52de8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="52de8-120">Authorization</span></span>  | <span data-ttu-id="52de8-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="52de8-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="52de8-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52de8-122">Request body</span></span>
<span data-ttu-id="52de8-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52de8-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="52de8-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="52de8-124">Parameter</span></span>    | <span data-ttu-id="52de8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="52de8-125">Type</span></span>   |<span data-ttu-id="52de8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="52de8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52de8-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="52de8-127">cancellationMessage</span></span>|<span data-ttu-id="52de8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52de8-128">String</span></span>|<span data-ttu-id="52de8-129">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="52de8-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="52de8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52de8-130">Response</span></span>
<span data-ttu-id="52de8-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52de8-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="52de8-133">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="52de8-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="52de8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52de8-134">Example</span></span>
<span data-ttu-id="52de8-135">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="52de8-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="52de8-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52de8-136">Request</span></span>
<span data-ttu-id="52de8-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52de8-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="52de8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="52de8-138">Response</span></span>
<span data-ttu-id="52de8-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52de8-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52de8-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="52de8-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52de8-141">Basic</span><span class="sxs-lookup"><span data-stu-id="52de8-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52de8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52de8-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingappointment_cancel-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
