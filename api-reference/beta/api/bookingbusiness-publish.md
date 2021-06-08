---
title: 'bookingBusiness: publish'
description: Disponibilizar a página de agendamento dessa empresa para clientes externos.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d60a88324cd86cd599fc9986dfa3b6d1a4f737ea
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786584"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="38dc5-103">bookingBusiness: publish</span><span class="sxs-lookup"><span data-stu-id="38dc5-103">bookingBusiness: publish</span></span>

<span data-ttu-id="38dc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38dc5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38dc5-105">Disponibilizar a página de agendamento dessa empresa para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="38dc5-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="38dc5-106">Defina a **propriedade isPublished** como true e **a propriedade publicUrl** como a URL da página de agendamento.</span><span class="sxs-lookup"><span data-stu-id="38dc5-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="38dc5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="38dc5-107">Permissions</span></span>
<span data-ttu-id="38dc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38dc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38dc5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38dc5-110">Permission type</span></span>      | <span data-ttu-id="38dc5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38dc5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38dc5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38dc5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="38dc5-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="38dc5-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="38dc5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38dc5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38dc5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38dc5-115">Not supported.</span></span>   |
|<span data-ttu-id="38dc5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38dc5-116">Application</span></span> | <span data-ttu-id="38dc5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38dc5-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="38dc5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38dc5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="38dc5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38dc5-119">Request headers</span></span>
| <span data-ttu-id="38dc5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="38dc5-120">Name</span></span>       | <span data-ttu-id="38dc5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38dc5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="38dc5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38dc5-122">Authorization</span></span>  | <span data-ttu-id="38dc5-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="38dc5-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="38dc5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38dc5-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="38dc5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="38dc5-125">Response</span></span>
<span data-ttu-id="38dc5-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38dc5-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38dc5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38dc5-128">Example</span></span>
<span data-ttu-id="38dc5-129">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="38dc5-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38dc5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38dc5-130">Request</span></span>
<span data-ttu-id="38dc5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38dc5-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38dc5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="38dc5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="38dc5-133">C#</span><span class="sxs-lookup"><span data-stu-id="38dc5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38dc5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38dc5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38dc5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38dc5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38dc5-136">Java</span><span class="sxs-lookup"><span data-stu-id="38dc5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38dc5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="38dc5-137">Response</span></span>
<span data-ttu-id="38dc5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38dc5-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


