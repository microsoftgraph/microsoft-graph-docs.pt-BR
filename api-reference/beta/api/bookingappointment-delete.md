---
title: Excluir bookingAppointment
description: Excluir um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e41f7c5df30ffd250d3efe032b8bea5d9503697f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960969"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="dacb8-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="dacb8-103">Delete bookingAppointment</span></span>

<span data-ttu-id="dacb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dacb8-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dacb8-105">Excluir um [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dacb8-105">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dacb8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dacb8-106">Permissions</span></span>
<span data-ttu-id="dacb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacb8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dacb8-109">Permission type</span></span>      | <span data-ttu-id="dacb8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dacb8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dacb8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dacb8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="dacb8-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="dacb8-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dacb8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dacb8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacb8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dacb8-114">Not supported.</span></span>   |
|<span data-ttu-id="dacb8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dacb8-115">Application</span></span> | <span data-ttu-id="dacb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dacb8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dacb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dacb8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="dacb8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dacb8-118">Request headers</span></span>
| <span data-ttu-id="dacb8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dacb8-119">Name</span></span>       | <span data-ttu-id="dacb8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dacb8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dacb8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dacb8-121">Authorization</span></span>  | <span data-ttu-id="dacb8-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="dacb8-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dacb8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dacb8-123">Request body</span></span>
<span data-ttu-id="dacb8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dacb8-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="dacb8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dacb8-125">Response</span></span>
<span data-ttu-id="dacb8-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dacb8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dacb8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dacb8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dacb8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dacb8-129">Request</span></span>
<span data-ttu-id="dacb8-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dacb8-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dacb8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="dacb8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="c"></a>[<span data-ttu-id="dacb8-132">C#</span><span class="sxs-lookup"><span data-stu-id="dacb8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dacb8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dacb8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dacb8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dacb8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dacb8-135">Java</span><span class="sxs-lookup"><span data-stu-id="dacb8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dacb8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dacb8-136">Response</span></span>
<span data-ttu-id="dacb8-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dacb8-137">The following is an example of the response.</span></span> <span data-ttu-id="dacb8-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="dacb8-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dacb8-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dacb8-139">All of the properties will be returned from an actual call.</span></span>
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


