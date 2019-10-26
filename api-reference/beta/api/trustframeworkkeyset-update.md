---
title: Atualizar trustFrameworkKeySet
description: Atualiza as propriedades de um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3de58ada2a4dd91042785366566b8f1ca2c907dc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734510"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="90ca9-103">Atualizar trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="90ca9-103">Update trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90ca9-104">Atualizar as propriedades de um [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="90ca9-104">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="90ca9-105">Essa operação substituirá o conteúdo de um conjunto de chaves existente.</span><span class="sxs-lookup"><span data-stu-id="90ca9-105">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="90ca9-106">A especificação da ID na carga de solicitação é opcional.</span><span class="sxs-lookup"><span data-stu-id="90ca9-106">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="90ca9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="90ca9-107">Permissions</span></span>

<span data-ttu-id="90ca9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90ca9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90ca9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90ca9-110">Permission type</span></span>                        | <span data-ttu-id="90ca9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90ca9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90ca9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90ca9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="90ca9-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90ca9-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="90ca9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90ca9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90ca9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90ca9-115">Not supported.</span></span> |
| <span data-ttu-id="90ca9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90ca9-116">Application</span></span>                            | <span data-ttu-id="90ca9-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="90ca9-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90ca9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90ca9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90ca9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca9-119">Request headers</span></span>

| <span data-ttu-id="90ca9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90ca9-120">Name</span></span>       | <span data-ttu-id="90ca9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ca9-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="90ca9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90ca9-122">Authorization</span></span> | <span data-ttu-id="90ca9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ca9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90ca9-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="90ca9-125">Content-type</span></span>  | <span data-ttu-id="90ca9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ca9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90ca9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca9-128">Request body</span></span>


| <span data-ttu-id="90ca9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90ca9-129">Property</span></span>     | <span data-ttu-id="90ca9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="90ca9-130">Type</span></span>        | <span data-ttu-id="90ca9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="90ca9-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90ca9-132">as</span><span class="sxs-lookup"><span data-stu-id="90ca9-132">keys</span></span>|<span data-ttu-id="90ca9-133">coleção [trustFrameworkKey](../resources/trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="90ca9-133">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="90ca9-134">atualiza uma coleção de Trustframeworkkeys</span><span class="sxs-lookup"><span data-stu-id="90ca9-134">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="90ca9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca9-135">Response</span></span>

<span data-ttu-id="90ca9-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca9-136">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90ca9-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90ca9-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90ca9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90ca9-138">Request</span></span>

<span data-ttu-id="90ca9-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90ca9-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}-->

```http
PUT https://graph.microsoft.com/beta/trustFramework/keySets/{id}
Content-type: application/json

{
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="90ca9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="90ca9-140">Response</span></span>

<span data-ttu-id="90ca9-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90ca9-141">The following is an example of the response.</span></span>

> <span data-ttu-id="90ca9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90ca9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update trustframeworkkeyset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
