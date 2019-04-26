---
title: 'bookingAppointment: cancelar'
description: Cancelar o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f80f97f6e085980d26ce4555f35f769db6a4f4e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322548"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="b1e34-103">bookingAppointment: cancelar</span><span class="sxs-lookup"><span data-stu-id="b1e34-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e34-104">Cancelar o [bookingAppointment](../resources/bookingappointment.md) especificado no [bookingbusiness](../resources/bookingbusiness.md)especificado e enviar uma mensagem para o cliente envolvido e os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="b1e34-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e34-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1e34-105">Permissions</span></span>
<span data-ttu-id="b1e34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e34-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1e34-108">Permission type</span></span>      | <span data-ttu-id="b1e34-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1e34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1e34-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1e34-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b1e34-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="b1e34-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b1e34-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1e34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1e34-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e34-113">Not supported.</span></span>   |
|<span data-ttu-id="b1e34-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1e34-114">Application</span></span> | <span data-ttu-id="b1e34-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1e34-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b1e34-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1e34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="b1e34-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e34-117">Request headers</span></span>
| <span data-ttu-id="b1e34-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b1e34-118">Name</span></span>       | <span data-ttu-id="b1e34-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e34-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b1e34-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1e34-120">Authorization</span></span>  | <span data-ttu-id="b1e34-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="b1e34-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1e34-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e34-122">Request body</span></span>
<span data-ttu-id="b1e34-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1e34-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1e34-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b1e34-124">Parameter</span></span>    | <span data-ttu-id="b1e34-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e34-125">Type</span></span>   |<span data-ttu-id="b1e34-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e34-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1e34-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="b1e34-127">cancellationMessage</span></span>|<span data-ttu-id="b1e34-128">String</span><span class="sxs-lookup"><span data-stu-id="b1e34-128">String</span></span>|<span data-ttu-id="b1e34-129">Uma mensagem a ser reconhecida pelo cliente de que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="b1e34-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="b1e34-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e34-130">Response</span></span>
<span data-ttu-id="b1e34-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e34-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="b1e34-133">Se você tentar cancelar um compromisso que não exisit, este método retornará `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="b1e34-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="b1e34-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1e34-134">Example</span></span>
<span data-ttu-id="b1e34-135">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b1e34-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b1e34-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1e34-136">Request</span></span>
<span data-ttu-id="b1e34-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1e34-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b1e34-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1e34-138">Response</span></span>
<span data-ttu-id="b1e34-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1e34-139">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
