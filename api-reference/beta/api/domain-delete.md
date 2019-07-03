---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f20c68bf95a1d60df27a8ae8412dd23cbf28a118
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436736"
---
# <a name="delete-domain"></a><span data-ttu-id="554aa-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="554aa-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="554aa-104">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="554aa-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="554aa-105">**Importante:** Os domínios excluídos não são recuperáveis.</span><span class="sxs-lookup"><span data-stu-id="554aa-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="554aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="554aa-106">Permissions</span></span>

<span data-ttu-id="554aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="554aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="554aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="554aa-109">Permission type</span></span>      | <span data-ttu-id="554aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="554aa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="554aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="554aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="554aa-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="554aa-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="554aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="554aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="554aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="554aa-114">Not supported.</span></span>    |
|<span data-ttu-id="554aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="554aa-115">Application</span></span> | <span data-ttu-id="554aa-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="554aa-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="554aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="554aa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="554aa-118">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="554aa-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="554aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="554aa-119">Request headers</span></span>

| <span data-ttu-id="554aa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="554aa-120">Name</span></span>       | <span data-ttu-id="554aa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="554aa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="554aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="554aa-122">Authorization</span></span>  | <span data-ttu-id="554aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="554aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="554aa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="554aa-125">Content-Type</span></span>  | <span data-ttu-id="554aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="554aa-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="554aa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="554aa-127">Request body</span></span>

<span data-ttu-id="554aa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="554aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="554aa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="554aa-129">Response</span></span>

<span data-ttu-id="554aa-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="554aa-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="554aa-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="554aa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="554aa-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="554aa-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="554aa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="554aa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="554aa-135">C#</span><span class="sxs-lookup"><span data-stu-id="554aa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="554aa-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="554aa-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="554aa-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="554aa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="554aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="554aa-138">Response</span></span>

<span data-ttu-id="554aa-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="554aa-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
