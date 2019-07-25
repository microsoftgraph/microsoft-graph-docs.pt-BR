---
title: Excluir bookingService
description: Exclua um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: ca96dc60ed0221cc58ddd5901ab3fd898033b0a8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865323"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="2b51b-103">Excluir bookingService</span><span class="sxs-lookup"><span data-stu-id="2b51b-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b51b-104">Exclua um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="2b51b-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2b51b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b51b-105">Permissions</span></span>
<span data-ttu-id="2b51b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b51b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b51b-108">Permission type</span></span>      | <span data-ttu-id="2b51b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b51b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b51b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b51b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b51b-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="2b51b-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2b51b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b51b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b51b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b51b-113">Not supported.</span></span>   |
|<span data-ttu-id="2b51b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b51b-114">Application</span></span> | <span data-ttu-id="2b51b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b51b-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2b51b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b51b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2b51b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b51b-117">Request headers</span></span>
| <span data-ttu-id="2b51b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2b51b-118">Name</span></span>       | <span data-ttu-id="2b51b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b51b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b51b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b51b-120">Authorization</span></span>  | <span data-ttu-id="2b51b-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2b51b-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b51b-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b51b-122">Request body</span></span>
<span data-ttu-id="2b51b-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b51b-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2b51b-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b51b-124">Response</span></span>
<span data-ttu-id="2b51b-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b51b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b51b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b51b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b51b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b51b-128">Request</span></span>
<span data-ttu-id="2b51b-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b51b-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b51b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b51b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b51b-131">C#</span><span class="sxs-lookup"><span data-stu-id="2b51b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b51b-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b51b-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b51b-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2b51b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2b51b-134">Java</span><span class="sxs-lookup"><span data-stu-id="2b51b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b51b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b51b-135">Response</span></span>
<span data-ttu-id="2b51b-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2b51b-136">The following is an example of the response.</span></span> <span data-ttu-id="2b51b-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="2b51b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2b51b-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b51b-138">All of the properties will be returned from an actual call.</span></span>
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
