---
title: Excluir reviewSetQuery
description: Excluir um objeto reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 8b400863cd9cbe6892f84f4c58d6b3ab738ddcb4
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509954"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="8d695-103">Excluir reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="8d695-103">Delete reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d695-104">Excluir um objeto [reviewSetQuery](../resources/reviewsetquery.md) .</span><span class="sxs-lookup"><span data-stu-id="8d695-104">Delete a [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d695-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d695-105">Permissions</span></span>

<span data-ttu-id="8d695-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d695-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d695-108">Permission type</span></span>                        | <span data-ttu-id="8d695-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d695-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d695-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d695-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d695-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="8d695-111">User.Read</span></span> |
| <span data-ttu-id="8d695-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d695-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d695-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d695-113">Not supported.</span></span> |
| <span data-ttu-id="8d695-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d695-114">Application</span></span>                            | <span data-ttu-id="8d695-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d695-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d695-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d695-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d695-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d695-117">Request headers</span></span>

| <span data-ttu-id="8d695-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8d695-118">Name</span></span>          | <span data-ttu-id="8d695-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d695-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d695-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d695-120">Authorization</span></span> | <span data-ttu-id="8d695-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d695-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d695-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d695-123">Request body</span></span>

<span data-ttu-id="8d695-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d695-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d695-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d695-125">Response</span></span>

<span data-ttu-id="8d695-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d695-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d695-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d695-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d695-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d695-129">Request</span></span>

<span data-ttu-id="8d695-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d695-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```

### <a name="response"></a><span data-ttu-id="8d695-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d695-131">Response</span></span>

<span data-ttu-id="8d695-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d695-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
