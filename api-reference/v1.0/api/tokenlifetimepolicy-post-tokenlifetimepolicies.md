---
title: Criar tokenLifetimePolicy
description: Criar um novo tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ffdf954ab963d123fca71c937d44add9a67cd53b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022966"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="affc0-103">Criar tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="affc0-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="affc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="affc0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="affc0-105">Criar um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="affc0-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="affc0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="affc0-106">Permissions</span></span>

<span data-ttu-id="affc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="affc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="affc0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="affc0-109">Permission type</span></span>                        | <span data-ttu-id="affc0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="affc0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="affc0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="affc0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="affc0-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="affc0-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="affc0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="affc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="affc0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="affc0-114">Not supported.</span></span> |
| <span data-ttu-id="affc0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="affc0-115">Application</span></span>                            | <span data-ttu-id="affc0-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="affc0-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="affc0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="affc0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="affc0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="affc0-118">Request headers</span></span>

| <span data-ttu-id="affc0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="affc0-119">Name</span></span>          | <span data-ttu-id="affc0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="affc0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="affc0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="affc0-121">Authorization</span></span> | <span data-ttu-id="affc0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="affc0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="affc0-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="affc0-124">Content-type</span></span> | <span data-ttu-id="affc0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="affc0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="affc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="affc0-127">Request body</span></span>

<span data-ttu-id="affc0-128">No corpo da solicitação, forneça uma representação JSON do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="affc0-128">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="affc0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="affc0-129">Response</span></span>

<span data-ttu-id="affc0-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="affc0-130">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="affc0-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="affc0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="affc0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="affc0-132">Request</span></span>

<span data-ttu-id="affc0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="affc0-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="affc0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="affc0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="affc0-135">C#</span><span class="sxs-lookup"><span data-stu-id="affc0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="affc0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="affc0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="affc0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="affc0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="affc0-138">Java</span><span class="sxs-lookup"><span data-stu-id="affc0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="affc0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="affc0-139">Response</span></span>

<span data-ttu-id="affc0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="affc0-140">The following is an example of the response.</span></span>

> <span data-ttu-id="affc0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="affc0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

