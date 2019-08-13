---
title: Excluir bookingAppointment
description: Excluir um bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 7166183eef43c7dc5b3ec7984073455e9110a212
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318450"
---
# <a name="delete-bookingappointment"></a><span data-ttu-id="4236c-103">Excluir bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="4236c-103">Delete bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4236c-104">Excluir um [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="4236c-104">Delete a [bookingAppointment](../resources/bookingappointment.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4236c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4236c-105">Permissions</span></span>
<span data-ttu-id="4236c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4236c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4236c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4236c-108">Permission type</span></span>      | <span data-ttu-id="4236c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4236c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4236c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4236c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4236c-111">BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="4236c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4236c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4236c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4236c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4236c-113">Not supported.</span></span>   |
|<span data-ttu-id="4236c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4236c-114">Application</span></span> | <span data-ttu-id="4236c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4236c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4236c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4236c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4236c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4236c-117">Request headers</span></span>
| <span data-ttu-id="4236c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4236c-118">Name</span></span>       | <span data-ttu-id="4236c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4236c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4236c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4236c-120">Authorization</span></span>  | <span data-ttu-id="4236c-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4236c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4236c-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4236c-122">Request body</span></span>
<span data-ttu-id="4236c-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4236c-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4236c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4236c-124">Response</span></span>
<span data-ttu-id="4236c-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4236c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4236c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4236c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4236c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4236c-128">Request</span></span>
<span data-ttu-id="4236c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4236c-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4236c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4236c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4236c-131">C#</span><span class="sxs-lookup"><span data-stu-id="4236c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4236c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4236c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4236c-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4236c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4236c-134">Java</span><span class="sxs-lookup"><span data-stu-id="4236c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4236c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4236c-135">Response</span></span>
<span data-ttu-id="4236c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4236c-136">The following is an example of the response.</span></span> <span data-ttu-id="4236c-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4236c-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4236c-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4236c-138">All of the properties will be returned from an actual call.</span></span>
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
