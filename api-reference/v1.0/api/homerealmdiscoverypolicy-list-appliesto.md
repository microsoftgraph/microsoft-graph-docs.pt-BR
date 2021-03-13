---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 68079092d20b35b0931c50b7610f1c8a3294baee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776113"
---
# <a name="list-appliesto"></a><span data-ttu-id="47d3b-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="47d3b-103">List appliesTo</span></span>

<span data-ttu-id="47d3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d3b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47d3b-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="47d3b-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="47d3b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="47d3b-106">Permissions</span></span>

<span data-ttu-id="47d3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47d3b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47d3b-109">Permission type</span></span>                        | <span data-ttu-id="47d3b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47d3b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47d3b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47d3b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47d3b-112">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="47d3b-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="47d3b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47d3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47d3b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47d3b-114">Not supported.</span></span> |
| <span data-ttu-id="47d3b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47d3b-115">Application</span></span>                            | <span data-ttu-id="47d3b-116">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="47d3b-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47d3b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47d3b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47d3b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47d3b-118">Optional query parameters</span></span>

<span data-ttu-id="47d3b-119">Este método dá suporte aos `$select` `$top` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47d3b-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="47d3b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47d3b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47d3b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47d3b-121">Request headers</span></span>

| <span data-ttu-id="47d3b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="47d3b-122">Name</span></span>      |<span data-ttu-id="47d3b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="47d3b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47d3b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="47d3b-124">Authorization</span></span> | <span data-ttu-id="47d3b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47d3b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47d3b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47d3b-127">Request body</span></span>

<span data-ttu-id="47d3b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47d3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47d3b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47d3b-129">Response</span></span>

<span data-ttu-id="47d3b-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47d3b-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47d3b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47d3b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47d3b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47d3b-132">Request</span></span>

<span data-ttu-id="47d3b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47d3b-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47d3b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="47d3b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="47d3b-135">C#</span><span class="sxs-lookup"><span data-stu-id="47d3b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47d3b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47d3b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47d3b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47d3b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47d3b-138">Java</span><span class="sxs-lookup"><span data-stu-id="47d3b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47d3b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="47d3b-139">Response</span></span>

<span data-ttu-id="47d3b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47d3b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="47d3b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47d3b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
