---
title: 'bookingAppointment: Cancelar'
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: ffb800b5084177b05b62e1ba14b475b8a760d766
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844475"
---
# <a name="bookingappointment-cancel"></a><span data-ttu-id="f9290-104">bookingAppointment: Cancelar</span><span class="sxs-lookup"><span data-stu-id="f9290-104">bookingAppointment: cancel</span></span>

 > <span data-ttu-id="f9290-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9290-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9290-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9290-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f9290-107">Cancele o [bookingAppointment](../resources/bookingappointment.md) especificado no especificado [bookingbusiness](../resources/bookingbusiness.md)e enviar uma mensagem para o cliente envolvido e a membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="f9290-107">Cancel the specified [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md), and send a message to the involved customer and staff members.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9290-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9290-108">Permissions</span></span>
<span data-ttu-id="f9290-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9290-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9290-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9290-111">Permission type</span></span>      | <span data-ttu-id="f9290-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9290-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9290-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9290-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f9290-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f9290-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f9290-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9290-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9290-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9290-116">Not supported.</span></span>   |
|<span data-ttu-id="f9290-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9290-117">Application</span></span> | <span data-ttu-id="f9290-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9290-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f9290-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9290-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a><span data-ttu-id="f9290-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9290-120">Request headers</span></span>
| <span data-ttu-id="f9290-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f9290-121">Name</span></span>       | <span data-ttu-id="f9290-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9290-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9290-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9290-123">Authorization</span></span>  | <span data-ttu-id="f9290-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f9290-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9290-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9290-125">Request body</span></span>
<span data-ttu-id="f9290-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9290-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9290-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9290-127">Parameter</span></span>    | <span data-ttu-id="f9290-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9290-128">Type</span></span>   |<span data-ttu-id="f9290-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9290-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9290-130">cancellationMessage</span><span class="sxs-lookup"><span data-stu-id="f9290-130">cancellationMessage</span></span>|<span data-ttu-id="f9290-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9290-131">String</span></span>|<span data-ttu-id="f9290-132">Uma mensagem de agradecer com o cliente que o compromisso foi cancelado.</span><span class="sxs-lookup"><span data-stu-id="f9290-132">A message to acknowledge with the customer that the appointment has been cancelled.</span></span>|

## <a name="response"></a><span data-ttu-id="f9290-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9290-133">Response</span></span>
<span data-ttu-id="f9290-p104">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9290-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="f9290-136">Se você tentar cancelar um compromisso que não não exisit, esse método retorna `HTTP 404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="f9290-136">If you attempt to cancel an appointment that does not exisit, this method returns `HTTP 404 Not found`.</span></span>

## <a name="example"></a><span data-ttu-id="f9290-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9290-137">Example</span></span>
<span data-ttu-id="f9290-138">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f9290-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9290-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9290-139">Request</span></span>
<span data-ttu-id="f9290-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9290-140">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f9290-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9290-141">Response</span></span>
<span data-ttu-id="f9290-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9290-142">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
