---
title: 'group: removeFavorite'
description: Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e01bd43238bee98658bea1acccee3a8876a3679c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885421"
---
# <a name="group-removefavorite"></a><span data-ttu-id="679f1-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="679f1-104">group: removeFavorite</span></span>
<span data-ttu-id="679f1-p102">Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="679f1-p102">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="679f1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="679f1-107">Permissions</span></span>
<span data-ttu-id="679f1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="679f1-110">Permission type</span></span>      | <span data-ttu-id="679f1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="679f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="679f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="679f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="679f1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679f1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="679f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="679f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="679f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679f1-115">Not supported.</span></span>    |
|<span data-ttu-id="679f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="679f1-116">Application</span></span> | <span data-ttu-id="679f1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679f1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="679f1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="679f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="679f1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="679f1-119">Request headers</span></span>
| <span data-ttu-id="679f1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="679f1-120">Header</span></span>       | <span data-ttu-id="679f1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="679f1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="679f1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="679f1-122">Authorization</span></span>  | <span data-ttu-id="679f1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679f1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="679f1-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="679f1-125">Prefer</span></span> | <span data-ttu-id="679f1-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="679f1-126">return=minimal.</span></span> <span data-ttu-id="679f1-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="679f1-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="679f1-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="679f1-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="679f1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="679f1-129">Request body</span></span>
<span data-ttu-id="679f1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="679f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="679f1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="679f1-131">Response</span></span>
<span data-ttu-id="679f1-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="679f1-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679f1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="679f1-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="679f1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679f1-135">Request</span></span>
<span data-ttu-id="679f1-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="679f1-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="679f1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="679f1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="679f1-138">C#</span><span class="sxs-lookup"><span data-stu-id="679f1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="679f1-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="679f1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="679f1-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="679f1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="679f1-141">Java</span><span class="sxs-lookup"><span data-stu-id="679f1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removefavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="679f1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="679f1-142">Response</span></span>
<span data-ttu-id="679f1-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="679f1-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
