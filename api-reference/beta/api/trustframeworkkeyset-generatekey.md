---
title: 'trustFrameworkKeySet: generateKey'
description: Gerar uma chave e um segredo automaticamente no conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c32501031d08e1b6d9dfc0fc78909e127a96b900
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734522"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="ddfbc-103">trustFrameworkKeySet: generateKey</span><span class="sxs-lookup"><span data-stu-id="ddfbc-103">trustFrameworkKeySet: generateKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddfbc-104">Gere um [trustFrameworkKey](../resources/trustFrameworkKey.md) e um segredo automaticamente no [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="ddfbc-104">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="ddfbc-105">O chamador não precisa fornecer um segredo.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-105">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddfbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddfbc-106">Permissions</span></span>

<span data-ttu-id="ddfbc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddfbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddfbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddfbc-109">Permission type</span></span>                        | <span data-ttu-id="ddfbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddfbc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddfbc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddfbc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddfbc-112">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddfbc-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="ddfbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddfbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddfbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-114">Not supported.</span></span> |
| <span data-ttu-id="ddfbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddfbc-115">Application</span></span>                            | <span data-ttu-id="ddfbc-116">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddfbc-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddfbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddfbc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="ddfbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfbc-118">Request headers</span></span>

| <span data-ttu-id="ddfbc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ddfbc-119">Name</span></span>          | <span data-ttu-id="ddfbc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddfbc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ddfbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddfbc-121">Authorization</span></span> | <span data-ttu-id="ddfbc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddfbc-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ddfbc-124">Content-type</span></span>  | <span data-ttu-id="ddfbc-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddfbc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfbc-127">Request body</span></span>

<span data-ttu-id="ddfbc-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ddfbc-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ddfbc-129">Parameter</span></span>    | <span data-ttu-id="ddfbc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddfbc-130">Type</span></span>        | <span data-ttu-id="ddfbc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddfbc-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ddfbc-132">Use</span><span class="sxs-lookup"><span data-stu-id="ddfbc-132">use</span></span> | <span data-ttu-id="ddfbc-133">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddfbc-133">string</span></span> | <span data-ttu-id="ddfbc-134">Semelhante à propriedade **use** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-134">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="ddfbc-135">kty</span><span class="sxs-lookup"><span data-stu-id="ddfbc-135">kty</span></span> | <span data-ttu-id="ddfbc-136">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddfbc-136">string</span></span> | <span data-ttu-id="ddfbc-137">Semelhante à propriedade **KTY** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-137">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="ddfbc-138">nbf</span><span class="sxs-lookup"><span data-stu-id="ddfbc-138">nbf</span></span> | <span data-ttu-id="ddfbc-139">int</span><span class="sxs-lookup"><span data-stu-id="ddfbc-139">int</span></span> | <span data-ttu-id="ddfbc-140">Semelhante à propriedade **NBF** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-140">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="ddfbc-141">exp</span><span class="sxs-lookup"><span data-stu-id="ddfbc-141">exp</span></span> | <span data-ttu-id="ddfbc-142">int</span><span class="sxs-lookup"><span data-stu-id="ddfbc-142">int</span></span> | <span data-ttu-id="ddfbc-143">Semelhante à propriedade **exp** de **trustFrameworkKey**.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-143">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="ddfbc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfbc-144">Response</span></span>

<span data-ttu-id="ddfbc-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-145">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddfbc-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddfbc-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddfbc-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddfbc-147">Request</span></span>

<span data-ttu-id="ddfbc-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/generateKey
Content-type: application/json

{
  "use": "sig",
  "kty": "RSA",
  "nbf": 1508969811,
  "exp": 1508969811
}
```

### <a name="response"></a><span data-ttu-id="ddfbc-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddfbc-149">Response</span></span>

<span data-ttu-id="ddfbc-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-150">The following is an example of the response.</span></span>

> <span data-ttu-id="ddfbc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddfbc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.trustFrameworkKey",
    "k": null,
    "x5c": [],
    "kty": "RSA",
    "use": "sig",
    "exp": 1908969811,
    "nbf": 1908969811,
    "kid": "Gaid7K8sO8RavMX9fzHir_Wg0femGhbY9b-B4rVIxbE",
    "e": "AQAB",
    "n": "rd54s6",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: generateKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
