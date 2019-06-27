---
title: 'bookingBusiness: publish'
description: Tornar a página de agendamento dessa empresa disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f533a9759db0b2e47c57b1ab55282804f4acf235
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257999"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="86623-103">bookingBusiness: publish</span><span class="sxs-lookup"><span data-stu-id="86623-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86623-104">Tornar a página de agendamento dessa empresa disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="86623-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="86623-105">Defina a \*\*\*\* Propriedade IsPublished como true e a propriedade **PUBLICURL** para a URL da página de agendamento.</span><span class="sxs-lookup"><span data-stu-id="86623-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="86623-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="86623-106">Permissions</span></span>
<span data-ttu-id="86623-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86623-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86623-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86623-109">Permission type</span></span>      | <span data-ttu-id="86623-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86623-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86623-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86623-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="86623-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="86623-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="86623-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86623-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86623-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86623-114">Not supported.</span></span>   |
|<span data-ttu-id="86623-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86623-115">Application</span></span> | <span data-ttu-id="86623-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86623-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="86623-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86623-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="86623-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86623-118">Request headers</span></span>
| <span data-ttu-id="86623-119">Nome</span><span class="sxs-lookup"><span data-stu-id="86623-119">Name</span></span>       | <span data-ttu-id="86623-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="86623-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="86623-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86623-121">Authorization</span></span>  | <span data-ttu-id="86623-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="86623-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="86623-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86623-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="86623-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="86623-124">Response</span></span>
<span data-ttu-id="86623-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86623-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86623-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86623-127">Example</span></span>
<span data-ttu-id="86623-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="86623-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="86623-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86623-129">Request</span></span>
<span data-ttu-id="86623-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86623-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="86623-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="86623-131">Response</span></span>
<span data-ttu-id="86623-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86623-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="86623-133">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="86623-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="86623-134">C#</span><span class="sxs-lookup"><span data-stu-id="86623-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86623-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="86623-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="86623-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="86623-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/bookingbusiness_publish-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
