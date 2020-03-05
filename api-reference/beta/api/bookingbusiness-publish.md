---
title: 'bookingBusiness: publish'
description: Tornar a página de agendamento dessa empresa disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b8ee635da938a53dff4603bb50f4903f0a000253
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441162"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="65612-103">bookingBusiness: publish</span><span class="sxs-lookup"><span data-stu-id="65612-103">bookingBusiness: publish</span></span>

<span data-ttu-id="65612-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65612-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65612-105">Tornar a página de agendamento dessa empresa disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="65612-105">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="65612-106">Defina a propriedade **IsPublished** como true e a propriedade **PUBLICURL** para a URL da página de agendamento.</span><span class="sxs-lookup"><span data-stu-id="65612-106">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="65612-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="65612-107">Permissions</span></span>
<span data-ttu-id="65612-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65612-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65612-110">Permission type</span></span>      | <span data-ttu-id="65612-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65612-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65612-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65612-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="65612-113">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="65612-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="65612-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65612-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65612-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65612-115">Not supported.</span></span>   |
|<span data-ttu-id="65612-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65612-116">Application</span></span> | <span data-ttu-id="65612-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65612-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="65612-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65612-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="65612-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65612-119">Request headers</span></span>
| <span data-ttu-id="65612-120">Nome</span><span class="sxs-lookup"><span data-stu-id="65612-120">Name</span></span>       | <span data-ttu-id="65612-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="65612-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="65612-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65612-122">Authorization</span></span>  | <span data-ttu-id="65612-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="65612-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="65612-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65612-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="65612-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="65612-125">Response</span></span>
<span data-ttu-id="65612-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65612-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65612-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65612-128">Example</span></span>
<span data-ttu-id="65612-129">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="65612-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="65612-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65612-130">Request</span></span>
<span data-ttu-id="65612-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65612-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65612-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="65612-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="c"></a>[<span data-ttu-id="65612-133">C#</span><span class="sxs-lookup"><span data-stu-id="65612-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65612-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65612-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65612-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65612-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65612-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="65612-136">Response</span></span>
<span data-ttu-id="65612-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65612-137">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
