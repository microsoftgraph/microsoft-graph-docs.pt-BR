---
title: Excluir bookingAppointment
description: Exclua um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 41a5096809b91ee25dfe8dc70071aa37c08aebb5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047935"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="2f947-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="2f947-103">Delete bookingAppointment</span></span>

<span data-ttu-id="2f947-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f947-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f947-105">Excluir um [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness especificado.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="2f947-105">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2f947-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f947-106">Permissions</span></span>
<span data-ttu-id="2f947-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f947-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f947-109">Permission type</span></span>      | <span data-ttu-id="2f947-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f947-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f947-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f947-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f947-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2f947-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2f947-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f947-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f947-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f947-114">Not supported.</span></span>   |
|<span data-ttu-id="2f947-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f947-115">Application</span></span> | <span data-ttu-id="2f947-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f947-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2f947-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f947-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2f947-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f947-118">Request headers</span></span>
| <span data-ttu-id="2f947-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2f947-119">Name</span></span>       | <span data-ttu-id="2f947-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f947-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f947-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f947-121">Authorization</span></span>  | <span data-ttu-id="2f947-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2f947-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f947-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f947-123">Request body</span></span>
<span data-ttu-id="2f947-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f947-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2f947-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f947-125">Response</span></span>
<span data-ttu-id="2f947-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f947-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f947-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f947-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f947-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f947-129">Request</span></span>
<span data-ttu-id="2f947-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f947-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f947-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f947-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="c"></a>[<span data-ttu-id="2f947-132">C#</span><span class="sxs-lookup"><span data-stu-id="2f947-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f947-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f947-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f947-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f947-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f947-135">Java</span><span class="sxs-lookup"><span data-stu-id="2f947-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2f947-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f947-136">Response</span></span>
<span data-ttu-id="2f947-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f947-137">The following is an example of the response.</span></span> <span data-ttu-id="2f947-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2f947-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


