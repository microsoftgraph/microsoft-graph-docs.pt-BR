---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c1bd1b7986062487ee9568ecfd0cbc0f5f020efc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945015"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="5ebbe-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="5ebbe-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ebbe-104">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="5ebbe-105">Defina a \*\*\*\* Propriedade IsPublished como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ebbe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ebbe-106">Permissions</span></span>
<span data-ttu-id="5ebbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ebbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ebbe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ebbe-109">Permission type</span></span>      | <span data-ttu-id="5ebbe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ebbe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ebbe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ebbe-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ebbe-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="5ebbe-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5ebbe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ebbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ebbe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-114">Not supported.</span></span>   |
|<span data-ttu-id="5ebbe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ebbe-115">Application</span></span> | <span data-ttu-id="5ebbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5ebbe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebbe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="5ebbe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebbe-118">Request headers</span></span>
| <span data-ttu-id="5ebbe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5ebbe-119">Name</span></span>       | <span data-ttu-id="5ebbe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ebbe-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ebbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebbe-121">Authorization</span></span>  | <span data-ttu-id="5ebbe-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5ebbe-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ebbe-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebbe-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5ebbe-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebbe-124">Response</span></span>
<span data-ttu-id="5ebbe-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ebbe-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ebbe-127">Example</span></span>
<span data-ttu-id="5ebbe-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ebbe-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ebbe-129">Request</span></span>
<span data-ttu-id="5ebbe-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5ebbe-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebbe-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ebbe-132">C#</span><span class="sxs-lookup"><span data-stu-id="5ebbe-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ebbe-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ebbe-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ebbe-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5ebbe-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5ebbe-135">Java</span><span class="sxs-lookup"><span data-stu-id="5ebbe-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-unpublish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ebbe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ebbe-136">Response</span></span>
<span data-ttu-id="5ebbe-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ebbe-137">The following is an example of the response.</span></span>
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
