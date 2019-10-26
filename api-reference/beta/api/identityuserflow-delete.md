---
title: Excluir userflow
description: Excluir userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 174cc8324b58c3a4deb627cd6f40bcbbab31f6a3
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734511"
---
# <a name="delete-userflow"></a><span data-ttu-id="adeab-103">Excluir userflow</span><span class="sxs-lookup"><span data-stu-id="adeab-103">Delete userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adeab-104">Excluir um objeto [userflow](../resources/identityuserflow.md) existente.</span><span class="sxs-lookup"><span data-stu-id="adeab-104">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adeab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="adeab-105">Permissions</span></span>

<span data-ttu-id="adeab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adeab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adeab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adeab-108">Permission type</span></span>                        | <span data-ttu-id="adeab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adeab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adeab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adeab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="adeab-111">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="adeab-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="adeab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adeab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adeab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="adeab-113">Not supported.</span></span> |
| <span data-ttu-id="adeab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adeab-114">Application</span></span>                            | <span data-ttu-id="adeab-115">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="adeab-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adeab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adeab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="adeab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adeab-117">Request headers</span></span>

| <span data-ttu-id="adeab-118">Nome</span><span class="sxs-lookup"><span data-stu-id="adeab-118">Name</span></span>          | <span data-ttu-id="adeab-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="adeab-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="adeab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="adeab-120">Authorization</span></span> | <span data-ttu-id="adeab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adeab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adeab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adeab-123">Request body</span></span>

<span data-ttu-id="adeab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adeab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adeab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="adeab-125">Response</span></span>

<span data-ttu-id="adeab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adeab-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adeab-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="adeab-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adeab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adeab-129">Request</span></span>

<span data-ttu-id="adeab-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="adeab-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```

### <a name="response"></a><span data-ttu-id="adeab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="adeab-131">Response</span></span>

<span data-ttu-id="adeab-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="adeab-132">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->