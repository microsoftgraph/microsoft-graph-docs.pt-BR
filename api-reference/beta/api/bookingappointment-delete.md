---
title: Excluir bookingAppointment
description: Excluir um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 708d6d0f40735844fd0e9badf916ec2dfd247832
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988125"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="4cc21-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="4cc21-103">Delete bookingAppointment</span></span>

<span data-ttu-id="4cc21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cc21-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cc21-105">Excluir um [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="4cc21-105">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4cc21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cc21-106">Permissions</span></span>
<span data-ttu-id="4cc21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cc21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cc21-109">Permission type</span></span>      | <span data-ttu-id="4cc21-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cc21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cc21-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cc21-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4cc21-112">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="4cc21-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4cc21-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cc21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cc21-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cc21-114">Not supported.</span></span>   |
|<span data-ttu-id="4cc21-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cc21-115">Application</span></span> | <span data-ttu-id="4cc21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cc21-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4cc21-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cc21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4cc21-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc21-118">Request headers</span></span>
| <span data-ttu-id="4cc21-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4cc21-119">Name</span></span>       | <span data-ttu-id="4cc21-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cc21-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4cc21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cc21-121">Authorization</span></span>  | <span data-ttu-id="4cc21-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4cc21-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cc21-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc21-123">Request body</span></span>
<span data-ttu-id="4cc21-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cc21-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4cc21-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc21-125">Response</span></span>
<span data-ttu-id="4cc21-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cc21-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cc21-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cc21-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cc21-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cc21-129">Request</span></span>
<span data-ttu-id="4cc21-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cc21-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cc21-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cc21-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="c"></a>[<span data-ttu-id="4cc21-132">C#</span><span class="sxs-lookup"><span data-stu-id="4cc21-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cc21-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cc21-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cc21-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cc21-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4cc21-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cc21-135">Response</span></span>
<span data-ttu-id="4cc21-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4cc21-136">The following is an example of the response.</span></span> <span data-ttu-id="4cc21-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4cc21-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4cc21-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cc21-138">All of the properties will be returned from an actual call.</span></span>
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


