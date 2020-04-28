---
title: Listar tokenLifetimePolicies
description: Obtenha uma lista de objetos tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d5b0aedc56f3e2f8fc366ec57aa6108fe0a83f8c
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917221"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="11986-103">Listar tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="11986-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="11986-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11986-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="11986-105">Obtenha uma lista de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11986-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="11986-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11986-106">Permissions</span></span>

<span data-ttu-id="11986-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11986-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11986-109">Permission type</span></span>                        | <span data-ttu-id="11986-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11986-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11986-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11986-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="11986-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11986-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="11986-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11986-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11986-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11986-114">Not supported.</span></span> |
| <span data-ttu-id="11986-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11986-115">Application</span></span>                            | <span data-ttu-id="11986-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11986-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="11986-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11986-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11986-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11986-118">Optional query parameters</span></span>

<span data-ttu-id="11986-119">Este método oferece suporte `$expand`a `$filter`, `$select` e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="11986-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="11986-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="11986-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="11986-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="11986-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11986-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11986-122">Request headers</span></span>

| <span data-ttu-id="11986-123">Nome</span><span class="sxs-lookup"><span data-stu-id="11986-123">Name</span></span>      |<span data-ttu-id="11986-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="11986-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11986-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="11986-125">Authorization</span></span> | <span data-ttu-id="11986-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11986-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11986-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11986-128">Request body</span></span>

<span data-ttu-id="11986-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11986-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11986-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="11986-130">Response</span></span>

<span data-ttu-id="11986-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11986-131">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11986-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11986-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11986-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11986-133">Request</span></span>

<span data-ttu-id="11986-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11986-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11986-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="11986-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="11986-136">C#</span><span class="sxs-lookup"><span data-stu-id="11986-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11986-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11986-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11986-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11986-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11986-139">Java</span><span class="sxs-lookup"><span data-stu-id="11986-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tokenlifetimepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11986-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="11986-140">Response</span></span>

<span data-ttu-id="11986-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11986-141">The following is an example of the response.</span></span>

> <span data-ttu-id="11986-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11986-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
