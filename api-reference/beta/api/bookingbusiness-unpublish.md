---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8d84d2b11895cd29b997a9049b31035956535426
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441148"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="9005a-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="9005a-103">bookingBusiness: unpublish</span></span>

<span data-ttu-id="9005a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9005a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9005a-105">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="9005a-105">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="9005a-106">Defina a propriedade **IsPublished** como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="9005a-106">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="9005a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9005a-107">Permissions</span></span>
<span data-ttu-id="9005a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9005a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9005a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9005a-110">Permission type</span></span>      | <span data-ttu-id="9005a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9005a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9005a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9005a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="9005a-113">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9005a-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9005a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9005a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9005a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9005a-115">Not supported.</span></span>   |
|<span data-ttu-id="9005a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9005a-116">Application</span></span> | <span data-ttu-id="9005a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9005a-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9005a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9005a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="9005a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9005a-119">Request headers</span></span>
| <span data-ttu-id="9005a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9005a-120">Name</span></span>       | <span data-ttu-id="9005a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9005a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9005a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9005a-122">Authorization</span></span>  | <span data-ttu-id="9005a-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9005a-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9005a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9005a-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9005a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9005a-125">Response</span></span>
<span data-ttu-id="9005a-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9005a-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9005a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9005a-128">Example</span></span>
<span data-ttu-id="9005a-129">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9005a-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9005a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9005a-130">Request</span></span>
<span data-ttu-id="9005a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9005a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9005a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9005a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="c"></a>[<span data-ttu-id="9005a-133">C#</span><span class="sxs-lookup"><span data-stu-id="9005a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9005a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9005a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9005a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9005a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9005a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9005a-136">Response</span></span>
<span data-ttu-id="9005a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9005a-137">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
