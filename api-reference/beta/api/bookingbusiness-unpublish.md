---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b56397200ffa0d450db6099540a4cfccb4c4339f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257929"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="1350f-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="1350f-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1350f-104">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="1350f-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="1350f-105">Defina a \*\*\*\* Propriedade IsPublished como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="1350f-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="1350f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1350f-106">Permissions</span></span>
<span data-ttu-id="1350f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1350f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1350f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1350f-109">Permission type</span></span>      | <span data-ttu-id="1350f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1350f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1350f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1350f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1350f-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="1350f-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1350f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1350f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1350f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1350f-114">Not supported.</span></span>   |
|<span data-ttu-id="1350f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1350f-115">Application</span></span> | <span data-ttu-id="1350f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1350f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1350f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1350f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="1350f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1350f-118">Request headers</span></span>
| <span data-ttu-id="1350f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1350f-119">Name</span></span>       | <span data-ttu-id="1350f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1350f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1350f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1350f-121">Authorization</span></span>  | <span data-ttu-id="1350f-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1350f-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1350f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1350f-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1350f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="1350f-124">Response</span></span>
<span data-ttu-id="1350f-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1350f-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1350f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1350f-127">Example</span></span>
<span data-ttu-id="1350f-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1350f-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1350f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1350f-129">Request</span></span>
<span data-ttu-id="1350f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1350f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="1350f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1350f-131">Response</span></span>
<span data-ttu-id="1350f-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1350f-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1350f-133">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="1350f-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1350f-134">C#</span><span class="sxs-lookup"><span data-stu-id="1350f-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1350f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1350f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1350f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1350f-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
