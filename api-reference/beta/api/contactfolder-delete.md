---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 192a5679449728c3dea6e46376427b3c47d5d229
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261296"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="a68a1-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="a68a1-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a68a1-104">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="a68a1-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a68a1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a68a1-105">Permissions</span></span>
<span data-ttu-id="a68a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a68a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a68a1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a68a1-108">Permission type</span></span>      | <span data-ttu-id="a68a1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a68a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a68a1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a68a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a68a1-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a68a1-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a68a1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a68a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a68a1-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a68a1-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a68a1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a68a1-114">Application</span></span> | <span data-ttu-id="a68a1-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a68a1-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a68a1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a68a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a68a1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a68a1-117">Request headers</span></span>
| <span data-ttu-id="a68a1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a68a1-118">Name</span></span>       | <span data-ttu-id="a68a1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a68a1-119">Type</span></span> | <span data-ttu-id="a68a1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a68a1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a68a1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a68a1-121">Authorization</span></span>  | <span data-ttu-id="a68a1-122">string</span><span class="sxs-lookup"><span data-stu-id="a68a1-122">string</span></span>  | <span data-ttu-id="a68a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a68a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a68a1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a68a1-125">Request body</span></span>
<span data-ttu-id="a68a1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a68a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a68a1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a68a1-127">Response</span></span>

<span data-ttu-id="a68a1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a68a1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a68a1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a68a1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a68a1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a68a1-131">Request</span></span>
<span data-ttu-id="a68a1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a68a1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="a68a1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a68a1-133">Response</span></span>
<span data-ttu-id="a68a1-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a68a1-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a68a1-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a68a1-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a68a1-136">C#</span><span class="sxs-lookup"><span data-stu-id="a68a1-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a68a1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a68a1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a68a1-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a68a1-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
