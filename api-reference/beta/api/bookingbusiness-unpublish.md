---
title: 'bookingBusiness: cancelar publicação'
description: Tornar a página de agendamento dessa empresa não disponível para clientes externos.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b32c2be3c7c318f7b26f1090892c5129e5634a51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987978"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="7365e-103">bookingBusiness: cancelar publicação</span><span class="sxs-lookup"><span data-stu-id="7365e-103">bookingBusiness: unpublish</span></span>

<span data-ttu-id="7365e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7365e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7365e-105">Tornar a página de agendamento dessa empresa não disponível para clientes externos.</span><span class="sxs-lookup"><span data-stu-id="7365e-105">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="7365e-106">Defina a propriedade **IsPublished** como false e a propriedade **publicUrl** como NULL.</span><span class="sxs-lookup"><span data-stu-id="7365e-106">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="7365e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7365e-107">Permissions</span></span>
<span data-ttu-id="7365e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7365e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7365e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7365e-110">Permission type</span></span>      | <span data-ttu-id="7365e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7365e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7365e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7365e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7365e-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7365e-113">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7365e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7365e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7365e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7365e-115">Not supported.</span></span>   |
|<span data-ttu-id="7365e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7365e-116">Application</span></span> | <span data-ttu-id="7365e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7365e-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7365e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7365e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="7365e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7365e-119">Request headers</span></span>
| <span data-ttu-id="7365e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7365e-120">Name</span></span>       | <span data-ttu-id="7365e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7365e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7365e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7365e-122">Authorization</span></span>  | <span data-ttu-id="7365e-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7365e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7365e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7365e-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7365e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="7365e-125">Response</span></span>
<span data-ttu-id="7365e-p102">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7365e-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7365e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7365e-128">Example</span></span>
<span data-ttu-id="7365e-129">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7365e-129">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7365e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7365e-130">Request</span></span>
<span data-ttu-id="7365e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7365e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7365e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7365e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```
# <a name="c"></a>[<span data-ttu-id="7365e-133">C#</span><span class="sxs-lookup"><span data-stu-id="7365e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-unpublish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7365e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7365e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-unpublish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7365e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7365e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-unpublish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7365e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7365e-136">Response</span></span>
<span data-ttu-id="7365e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7365e-137">The following is an example of the response.</span></span>
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


