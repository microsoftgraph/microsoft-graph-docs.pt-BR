---
title: Excluir bookingService
description: Exclua um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c7ba9cb20e7f9f401d7b9651d408549272b32875
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047809"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="63bab-103">Excluir bookingService</span><span class="sxs-lookup"><span data-stu-id="63bab-103">Delete bookingService</span></span>

<span data-ttu-id="63bab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63bab-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63bab-105">[Exclua um objeto bookingService](../resources/bookingservice.md) no [bookingbusiness especificado.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="63bab-105">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="63bab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63bab-106">Permissions</span></span>
<span data-ttu-id="63bab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63bab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63bab-109">Permission type</span></span>      | <span data-ttu-id="63bab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63bab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63bab-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63bab-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="63bab-112">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="63bab-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="63bab-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63bab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63bab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bab-114">Not supported.</span></span>   |
|<span data-ttu-id="63bab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63bab-115">Application</span></span> | <span data-ttu-id="63bab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63bab-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63bab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63bab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="63bab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63bab-118">Request headers</span></span>
| <span data-ttu-id="63bab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="63bab-119">Name</span></span>       | <span data-ttu-id="63bab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63bab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63bab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="63bab-121">Authorization</span></span>  | <span data-ttu-id="63bab-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="63bab-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="63bab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63bab-123">Request body</span></span>
<span data-ttu-id="63bab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63bab-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="63bab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bab-125">Response</span></span>
<span data-ttu-id="63bab-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63bab-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63bab-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63bab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63bab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63bab-129">Request</span></span>
<span data-ttu-id="63bab-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="63bab-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63bab-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="63bab-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="63bab-132">C#</span><span class="sxs-lookup"><span data-stu-id="63bab-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63bab-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63bab-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63bab-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63bab-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63bab-135">Java</span><span class="sxs-lookup"><span data-stu-id="63bab-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63bab-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="63bab-136">Response</span></span>
<span data-ttu-id="63bab-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="63bab-137">The following is an example of the response.</span></span> <span data-ttu-id="63bab-138">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="63bab-138">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


