---
title: Excluir trustFrameworkKeySet
description: Excluir um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad73363f568c97be720cdcab3711e762b8dcde1a
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734515"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="547a9-103">Excluir trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="547a9-103">Delete trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="547a9-104">Excluir um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="547a9-104">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="547a9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="547a9-105">Permissions</span></span>

<span data-ttu-id="547a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="547a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="547a9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="547a9-108">Permission type</span></span>                        | <span data-ttu-id="547a9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="547a9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="547a9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="547a9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="547a9-111">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="547a9-111">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="547a9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="547a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="547a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="547a9-113">Not supported.</span></span> |
| <span data-ttu-id="547a9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="547a9-114">Application</span></span>                            | <span data-ttu-id="547a9-115">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="547a9-115">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="547a9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="547a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="547a9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="547a9-117">Request headers</span></span>

| <span data-ttu-id="547a9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="547a9-118">Name</span></span>          | <span data-ttu-id="547a9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="547a9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="547a9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="547a9-120">Authorization</span></span> | <span data-ttu-id="547a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="547a9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="547a9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="547a9-123">Request body</span></span>

<span data-ttu-id="547a9-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="547a9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="547a9-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="547a9-125">Response</span></span>

<span data-ttu-id="547a9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="547a9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="547a9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="547a9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="547a9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="547a9-129">Request</span></span>

<span data-ttu-id="547a9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="547a9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="547a9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="547a9-131">Response</span></span>

<span data-ttu-id="547a9-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="547a9-132">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
