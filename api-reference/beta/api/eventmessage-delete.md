---
title: Excluir eventMessage
description: Exclua a eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e0ea2f13edbaeb77cfff7a0e84820a473a5e7395
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259147"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="8ae02-103">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="8ae02-103">Delete eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ae02-104">Exclua a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="8ae02-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ae02-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ae02-105">Permissions</span></span>
<span data-ttu-id="8ae02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae02-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ae02-108">Permission type</span></span>      | <span data-ttu-id="8ae02-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ae02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ae02-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ae02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ae02-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ae02-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ae02-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ae02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ae02-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ae02-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ae02-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ae02-114">Application</span></span> | <span data-ttu-id="8ae02-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ae02-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ae02-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ae02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ae02-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae02-117">Request headers</span></span>
| <span data-ttu-id="8ae02-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8ae02-118">Name</span></span>       | <span data-ttu-id="8ae02-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ae02-119">Type</span></span> | <span data-ttu-id="8ae02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ae02-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ae02-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ae02-121">Authorization</span></span>  | <span data-ttu-id="8ae02-122">string</span><span class="sxs-lookup"><span data-stu-id="8ae02-122">string</span></span>  | <span data-ttu-id="8ae02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ae02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ae02-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae02-125">Request body</span></span>
<span data-ttu-id="8ae02-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ae02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ae02-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae02-127">Response</span></span>

<span data-ttu-id="8ae02-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ae02-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae02-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ae02-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ae02-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae02-131">Request</span></span>
<span data-ttu-id="8ae02-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ae02-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="8ae02-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae02-133">Response</span></span>
<span data-ttu-id="8ae02-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ae02-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8ae02-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8ae02-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8ae02-136">C#</span><span class="sxs-lookup"><span data-stu-id="8ae02-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ae02-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ae02-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8ae02-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8ae02-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/eventmessage-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
