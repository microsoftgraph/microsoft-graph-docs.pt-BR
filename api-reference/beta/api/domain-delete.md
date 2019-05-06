---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f249c17fc296b85bc45c8d8eed620b1742b1b55b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589375"
---
# <a name="delete-domain"></a><span data-ttu-id="fe7d1-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="fe7d1-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe7d1-104">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="fe7d1-105">**Importante:** Os domínios excluídos não são recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe7d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe7d1-106">Permissions</span></span>

<span data-ttu-id="fe7d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe7d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fe7d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe7d1-109">Permission type</span></span>      | <span data-ttu-id="fe7d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe7d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe7d1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe7d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe7d1-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe7d1-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe7d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe7d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe7d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-114">Not supported.</span></span>    |
|<span data-ttu-id="fe7d1-115">Application</span><span class="sxs-lookup"><span data-stu-id="fe7d1-115">Application</span></span> | <span data-ttu-id="fe7d1-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe7d1-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe7d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe7d1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="fe7d1-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe7d1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7d1-119">Request headers</span></span>

| <span data-ttu-id="fe7d1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fe7d1-120">Name</span></span>       | <span data-ttu-id="fe7d1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe7d1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe7d1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe7d1-122">Authorization</span></span>  | <span data-ttu-id="fe7d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe7d1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe7d1-125">Content-Type</span></span>  | <span data-ttu-id="fe7d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe7d1-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe7d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7d1-127">Request body</span></span>

<span data-ttu-id="fe7d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe7d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7d1-129">Response</span></span>

<span data-ttu-id="fe7d1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe7d1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe7d1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe7d1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe7d1-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="fe7d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe7d1-134">Response</span></span>

<span data-ttu-id="fe7d1-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe7d1-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fe7d1-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fe7d1-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fe7d1-138">Basic</span><span class="sxs-lookup"><span data-stu-id="fe7d1-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe7d1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe7d1-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
