---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dc0d94094273579321a614c9ff2192f331550421
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636188"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="aa284-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="aa284-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa284-104">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="aa284-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="aa284-105">Defina a \*\*\*\* Propriedade IsPublished como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="aa284-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa284-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa284-106">Permissions</span></span>
<span data-ttu-id="aa284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa284-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa284-109">Permission type</span></span>      | <span data-ttu-id="aa284-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa284-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa284-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa284-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="aa284-112">Bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="aa284-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="aa284-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa284-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa284-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa284-114">Not supported.</span></span>   |
|<span data-ttu-id="aa284-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa284-115">Application</span></span> | <span data-ttu-id="aa284-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa284-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="aa284-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa284-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="aa284-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa284-118">Request headers</span></span>
| <span data-ttu-id="aa284-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aa284-119">Name</span></span>       | <span data-ttu-id="aa284-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa284-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa284-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa284-121">Authorization</span></span>  | <span data-ttu-id="aa284-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="aa284-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa284-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa284-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="aa284-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa284-124">Response</span></span>
<span data-ttu-id="aa284-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa284-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa284-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa284-127">Example</span></span>
<span data-ttu-id="aa284-128">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aa284-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa284-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa284-129">Request</span></span>
<span data-ttu-id="aa284-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa284-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="aa284-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa284-131">Response</span></span>
<span data-ttu-id="aa284-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa284-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aa284-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="aa284-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aa284-134">Basic</span><span class="sxs-lookup"><span data-stu-id="aa284-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa284-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa284-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/bookingbusiness_unpublish-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
