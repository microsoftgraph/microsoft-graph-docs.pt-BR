---
title: Criar tokenLifetimePolicy
description: Criar um novo tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d40146e205dd250f99df3334b5e0c8d0323564c7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234112"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="a45c3-103">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a45c3-103">Create tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a45c3-104">Criar um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a45c3-104">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a45c3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a45c3-105">Permissions</span></span>

<span data-ttu-id="a45c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a45c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a45c3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a45c3-108">Permission type</span></span>                        | <span data-ttu-id="a45c3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a45c3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a45c3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a45c3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a45c3-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a45c3-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a45c3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a45c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a45c3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a45c3-113">Not supported.</span></span> |
| <span data-ttu-id="a45c3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a45c3-114">Application</span></span>                            | <span data-ttu-id="a45c3-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a45c3-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a45c3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a45c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a45c3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a45c3-117">Request headers</span></span>

| <span data-ttu-id="a45c3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a45c3-118">Name</span></span>          | <span data-ttu-id="a45c3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a45c3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a45c3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a45c3-120">Authorization</span></span> | <span data-ttu-id="a45c3-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a45c3-121">Bearer {token}</span></span> |
| <span data-ttu-id="a45c3-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="a45c3-122">Content-type</span></span> | <span data-ttu-id="a45c3-123">application/json</span><span class="sxs-lookup"><span data-stu-id="a45c3-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a45c3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a45c3-124">Request body</span></span>

<span data-ttu-id="a45c3-125">No corpo da solicitação, forneça uma representação JSON do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a45c3-125">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a45c3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a45c3-126">Response</span></span>

<span data-ttu-id="a45c3-127">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a45c3-127">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a45c3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a45c3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a45c3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a45c3-129">Request</span></span>

<span data-ttu-id="a45c3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a45c3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="a45c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a45c3-131">Response</span></span>

<span data-ttu-id="a45c3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a45c3-132">The following is an example of the response.</span></span>

> <span data-ttu-id="a45c3-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a45c3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->