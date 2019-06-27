---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0921a946ce0b22a49a978530981184c06fbf84a3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260715"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="8297e-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="8297e-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8297e-104">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="8297e-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="8297e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8297e-105">Permissions</span></span>

<span data-ttu-id="8297e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8297e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8297e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8297e-108">Permission type</span></span>      | <span data-ttu-id="8297e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8297e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8297e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8297e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8297e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8297e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8297e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8297e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8297e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8297e-113">Not supported.</span></span>    |
|<span data-ttu-id="8297e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8297e-114">Application</span></span> | <span data-ttu-id="8297e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8297e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8297e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8297e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8297e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8297e-117">Request headers</span></span>

| <span data-ttu-id="8297e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8297e-118">Name</span></span>       | <span data-ttu-id="8297e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8297e-119">Type</span></span> | <span data-ttu-id="8297e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8297e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8297e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8297e-121">Authorization</span></span>  | <span data-ttu-id="8297e-122">string</span><span class="sxs-lookup"><span data-stu-id="8297e-122">string</span></span>  | <span data-ttu-id="8297e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8297e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8297e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8297e-125">Request body</span></span>

<span data-ttu-id="8297e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8297e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8297e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8297e-127">Response</span></span>

<span data-ttu-id="8297e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8297e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8297e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8297e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8297e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8297e-131">Request</span></span>

<span data-ttu-id="8297e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8297e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="8297e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8297e-133">Response</span></span>

<span data-ttu-id="8297e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8297e-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8297e-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8297e-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8297e-136">C#</span><span class="sxs-lookup"><span data-stu-id="8297e-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8297e-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8297e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8297e-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8297e-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
