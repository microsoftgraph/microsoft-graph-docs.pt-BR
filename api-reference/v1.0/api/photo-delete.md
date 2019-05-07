---
title: Excluir foto
description: Exclua uma foto.
localization_priority: Normal
ms.openlocfilehash: 05a679217aea32ee026ef1786c7d6a21689d1cab
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611409"
---
# <a name="delete-photo"></a><span data-ttu-id="bb15a-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="bb15a-103">Delete photo</span></span>

<span data-ttu-id="bb15a-104">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="bb15a-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb15a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb15a-105">Permissions</span></span>
<span data-ttu-id="bb15a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb15a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb15a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb15a-108">Permission type</span></span>      | <span data-ttu-id="bb15a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb15a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb15a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb15a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb15a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb15a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb15a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb15a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb15a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb15a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb15a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb15a-114">Application</span></span> | <span data-ttu-id="bb15a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb15a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb15a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb15a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="bb15a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb15a-117">Request headers</span></span>
| <span data-ttu-id="bb15a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bb15a-118">Name</span></span>       | <span data-ttu-id="bb15a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb15a-119">Type</span></span> | <span data-ttu-id="bb15a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb15a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb15a-121">if-match</span><span class="sxs-lookup"><span data-stu-id="bb15a-121">if-match</span></span>  | <span data-ttu-id="bb15a-122">string</span><span class="sxs-lookup"><span data-stu-id="bb15a-122">string</span></span>  | <span data-ttu-id="bb15a-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="bb15a-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="bb15a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb15a-124">Authorization</span></span>  | <span data-ttu-id="bb15a-125">string</span><span class="sxs-lookup"><span data-stu-id="bb15a-125">string</span></span>  | <span data-ttu-id="bb15a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb15a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb15a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb15a-128">Request body</span></span>
<span data-ttu-id="bb15a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb15a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb15a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb15a-130">Response</span></span>

<span data-ttu-id="bb15a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb15a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb15a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb15a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb15a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb15a-134">Request</span></span>
<span data-ttu-id="bb15a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb15a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="bb15a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb15a-136">Response</span></span>
<span data-ttu-id="bb15a-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb15a-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb15a-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bb15a-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb15a-139">Basic</span><span class="sxs-lookup"><span data-stu-id="bb15a-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb15a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb15a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_photo-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/photo-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
