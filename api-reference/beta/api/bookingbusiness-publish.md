---
title: 'bookingBusiness: publish'
description: Tornar a página de agendamento dessa empresa disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8d6904b48f4cfc57ab344b6bf58c26de3ca612b3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439144"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="5dc28-103">bookingBusiness: publish</span><span class="sxs-lookup"><span data-stu-id="5dc28-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc28-104">Tornar a página de agendamento dessa empresa disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="5dc28-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="5dc28-105">Defina a \*\*\*\* Propriedade IsPublished como true e a propriedade **PUBLICURL** para a URL da página de agendamento.</span><span class="sxs-lookup"><span data-stu-id="5dc28-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dc28-106">Permissions</span></span>
<span data-ttu-id="5dc28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc28-109">Permission type</span></span>      | <span data-ttu-id="5dc28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dc28-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dc28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc28-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5dc28-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="5dc28-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5dc28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc28-114">Not supported.</span></span>   |
|<span data-ttu-id="5dc28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc28-115">Application</span></span> | <span data-ttu-id="5dc28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc28-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5dc28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc28-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="5dc28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc28-118">Request headers</span></span>
| <span data-ttu-id="5dc28-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5dc28-119">Name</span></span>       | <span data-ttu-id="5dc28-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc28-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5dc28-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dc28-121">Authorization</span></span>  | <span data-ttu-id="5dc28-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5dc28-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc28-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc28-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5dc28-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc28-124">Response</span></span>
<span data-ttu-id="5dc28-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc28-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc28-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc28-127">Example</span></span>
<span data-ttu-id="5dc28-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5dc28-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5dc28-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc28-129">Request</span></span>
<span data-ttu-id="5dc28-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc28-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5dc28-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc28-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5dc28-132">C#</span><span class="sxs-lookup"><span data-stu-id="5dc28-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dc28-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dc28-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5dc28-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5dc28-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5dc28-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc28-135">Response</span></span>
<span data-ttu-id="5dc28-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc28-136">The following is an example of the response.</span></span>
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
