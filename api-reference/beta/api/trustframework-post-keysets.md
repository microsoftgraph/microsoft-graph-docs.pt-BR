---
title: Criar trustFrameworkKeySet
description: Criar um novo objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b6cd03a38e4e115befacb13909d1ba0040b3aff
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734523"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="f588c-103">Criar trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="f588c-103">Create trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f588c-104">Criar um novo [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="f588c-104">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="f588c-105">A ID do **trustFrameworkKeySet** é esperada na solicitação Create; no entanto, ele pode ser modificado pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="f588c-105">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="f588c-106">O ID modificado estará disponível na resposta e no cabeçalho do local.</span><span class="sxs-lookup"><span data-stu-id="f588c-106">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="f588c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f588c-107">Permissions</span></span>

<span data-ttu-id="f588c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f588c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f588c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f588c-110">Permission type</span></span>                        | <span data-ttu-id="f588c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f588c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f588c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f588c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f588c-113">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f588c-113">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="f588c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f588c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f588c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f588c-115">Not supported.</span></span> |
| <span data-ttu-id="f588c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f588c-116">Application</span></span>                            | <span data-ttu-id="f588c-117">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f588c-117">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="f588c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f588c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="f588c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f588c-119">Request headers</span></span>

| <span data-ttu-id="f588c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f588c-120">Name</span></span>          | <span data-ttu-id="f588c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f588c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f588c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f588c-122">Authorization</span></span> | <span data-ttu-id="f588c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f588c-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f588c-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f588c-125">Content-type</span></span> | <span data-ttu-id="f588c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f588c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f588c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f588c-128">Request body</span></span>

<span data-ttu-id="f588c-129">No corpo da solicitação, forneça uma representação JSON de um objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) .</span><span class="sxs-lookup"><span data-stu-id="f588c-129">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f588c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f588c-130">Response</span></span>

<span data-ttu-id="f588c-131">Se tiver êxito, este método retornará `201 Created` um código de resposta, um cabeçalho de local para o objeto recém-criado e um novo objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f588c-131">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f588c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f588c-132">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="f588c-133">Exemplo 1: criar um conjunto de chaves vazio</span><span class="sxs-lookup"><span data-stu-id="f588c-133">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="f588c-134">Este padrão para criar um conjunto de chaves enpty e, em seguida, gerar uma chave, carregar um segredo manual e carregar um certificado ou uma chave PKCS12 é suficiente para a maioria dos cenários.</span><span class="sxs-lookup"><span data-stu-id="f588c-134">This pattern to create an enpty keyset and then generate a key, upload a manual secret, and upload a certificate or a PKCS12 key is sufficient for most scenarios.</span></span> 

#### <a name="request"></a><span data-ttu-id="f588c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f588c-135">Request</span></span>

<span data-ttu-id="f588c-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f588c-136">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework1"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1"  
}
```

#### <a name="response"></a><span data-ttu-id="f588c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f588c-137">Response</span></span>

<span data-ttu-id="f588c-138">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f588c-138">The following example shows the response.</span></span>

> <span data-ttu-id="f588c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f588c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": []
}
```

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="f588c-141">Exemplo 2: criar um conjunto de chaves com uma chave</span><span class="sxs-lookup"><span data-stu-id="f588c-141">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="f588c-142">Este é um cenário avançado onde você precisa saber o formato de chave da Web JSON compatível com [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) da chave.</span><span class="sxs-lookup"><span data-stu-id="f588c-142">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="f588c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f588c-143">Request</span></span>

<span data-ttu-id="f588c-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f588c-144">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1",
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

#### <a name="response"></a><span data-ttu-id="f588c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f588c-145">Response</span></span>

<span data-ttu-id="f588c-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f588c-146">The following example shows the response.</span></span>

> <span data-ttu-id="f588c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f588c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
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
  "description": "Create trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
