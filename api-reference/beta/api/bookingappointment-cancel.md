---
title: 'bookingAppointment: Cancelar'
description: Cancele o bookingAppointment especificado no bookingbusiness especificado e enviar uma mensagem para os membros da equipe e cliente envolvidos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c202ea309641bdcda3e1124792fdc04ad97e02ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514681"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="6cc40-103">bookingAppointment: Cancelar</span><span class="sxs-lookup"><span data-stu-id="6cc40-103">bookingAppointment: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cc40-104">Cancele o [bookingAppointment](../resources/bookingappointment.md) especificado no especificado [bookingbusiness](../resources/bookingbusiness.md)e enviar uma mensagem para o cliente envolvido e a membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="6cc40-104">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cc40-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cc40-105">Permissions</span></span>
<span data-ttu-id="6cc40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc40-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cc40-108">Permission type</span></span>      | <span data-ttu-id="6cc40-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cc40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cc40-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cc40-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6cc40-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6cc40-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6cc40-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cc40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cc40-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc40-113">Not supported.</span></span>   |
|<span data-ttu-id="6cc40-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cc40-114">Application</span></span> | <span data-ttu-id="6cc40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cc40-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6cc40-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cc40-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="6cc40-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc40-117">Request headers</span></span>
| <span data-ttu-id="6cc40-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6cc40-118">Name</span></span>       | <span data-ttu-id="6cc40-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc40-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6cc40-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cc40-120">Authorization</span></span>  | <span data-ttu-id="6cc40-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="6cc40-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc40-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc40-122">Request body</span></span>
<span data-ttu-id="6cc40-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc40-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cc40-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6cc40-124">Parameter</span></span>    | <span data-ttu-id="6cc40-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cc40-125">Type</span></span>   |<span data-ttu-id="6cc40-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cc40-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cc40-127">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="6cc40-127">cancellationMessage</span></span>|<span data-ttu-id="6cc40-128">String</span><span class="sxs-lookup"><span data-stu-id="6cc40-128">String</span></span>|<span data-ttu-id="6cc40-129">Uma mensagem de agradecer com o cliente que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="6cc40-129">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="6cc40-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc40-130">Response</span></span>
<span data-ttu-id="6cc40-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc40-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="6cc40-133">Se você tentar cancelar um compromisso que não não exisit, esse método retorna `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="6cc40-133">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="6cc40-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cc40-134">Example</span></span>
<span data-ttu-id="6cc40-135">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6cc40-135">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6cc40-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cc40-136">Request</span></span>
<span data-ttu-id="6cc40-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cc40-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6cc40-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cc40-138">Response</span></span>
<span data-ttu-id="6cc40-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6cc40-139">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingappointment-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
