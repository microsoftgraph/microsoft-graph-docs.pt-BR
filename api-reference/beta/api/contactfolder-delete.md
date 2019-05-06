---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9ff9837b112f17c85edd2d382c46d9d8c1f22329
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591437"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="42eaf-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="42eaf-103">Delete contactFolder</span></span>

<span data-ttu-id="42eaf-104">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="42eaf-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="42eaf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="42eaf-105">Permissions</span></span>
<span data-ttu-id="42eaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42eaf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42eaf-108">Permission type</span></span>      | <span data-ttu-id="42eaf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42eaf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42eaf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42eaf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42eaf-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42eaf-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="42eaf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42eaf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42eaf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42eaf-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="42eaf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42eaf-114">Application</span></span> | <span data-ttu-id="42eaf-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42eaf-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42eaf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42eaf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="42eaf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42eaf-117">Request headers</span></span>
| <span data-ttu-id="42eaf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="42eaf-118">Name</span></span>       | <span data-ttu-id="42eaf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="42eaf-119">Type</span></span> | <span data-ttu-id="42eaf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42eaf-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42eaf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42eaf-121">Authorization</span></span>  | <span data-ttu-id="42eaf-122">string</span><span class="sxs-lookup"><span data-stu-id="42eaf-122">string</span></span>  | <span data-ttu-id="42eaf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42eaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42eaf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42eaf-125">Request body</span></span>
<span data-ttu-id="42eaf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42eaf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42eaf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="42eaf-127">Response</span></span>

<span data-ttu-id="42eaf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42eaf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42eaf-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42eaf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42eaf-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42eaf-131">Request</span></span>
<span data-ttu-id="42eaf-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42eaf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="42eaf-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42eaf-133">Response</span></span>
<span data-ttu-id="42eaf-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42eaf-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="42eaf-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="42eaf-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="42eaf-136">Basic</span><span class="sxs-lookup"><span data-stu-id="42eaf-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42eaf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42eaf-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contactfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contactfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
