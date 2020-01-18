---
title: Excluir tokenLifetimePolicy
description: Exclua tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cb4944beb5057bec0098556f81292f4ed9202910
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234095"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="8d865-103">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="8d865-103">Delete tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d865-104">Excluir um objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8d865-104">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d865-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d865-105">Permissions</span></span>

<span data-ttu-id="8d865-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d865-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d865-108">Permission type</span></span>                        | <span data-ttu-id="8d865-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d865-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d865-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d865-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d865-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d865-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8d865-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d865-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d865-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d865-113">Not supported.</span></span> |
| <span data-ttu-id="8d865-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d865-114">Application</span></span>                            | <span data-ttu-id="8d865-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d865-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d865-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d865-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d865-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d865-117">Request headers</span></span>

| <span data-ttu-id="8d865-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8d865-118">Name</span></span>          | <span data-ttu-id="8d865-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d865-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d865-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d865-120">Authorization</span></span> | <span data-ttu-id="8d865-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8d865-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d865-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d865-122">Request body</span></span>

<span data-ttu-id="8d865-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d865-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d865-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d865-124">Response</span></span>

<span data-ttu-id="8d865-125">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d865-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8d865-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d865-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d865-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d865-127">Request</span></span>

<span data-ttu-id="8d865-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d865-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="8d865-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d865-129">Response</span></span>

<span data-ttu-id="8d865-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d865-130">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->