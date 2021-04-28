---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3c30809b8dd25960dbe26275df2509d848a9063a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051400"
---
# <a name="list-appliesto"></a><span data-ttu-id="324d1-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="324d1-103">List appliesTo</span></span>

<span data-ttu-id="324d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="324d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="324d1-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="324d1-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="324d1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="324d1-106">Permissions</span></span>

<span data-ttu-id="324d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="324d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="324d1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="324d1-109">Permission type</span></span>                        | <span data-ttu-id="324d1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="324d1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="324d1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="324d1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="324d1-112">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="324d1-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="324d1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="324d1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="324d1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="324d1-114">Not supported.</span></span> |
| <span data-ttu-id="324d1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="324d1-115">Application</span></span>                            | <span data-ttu-id="324d1-116">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="324d1-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="324d1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="324d1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="324d1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="324d1-118">Optional query parameters</span></span>

<span data-ttu-id="324d1-119">Este método dá suporte aos `$select` `$top` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="324d1-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="324d1-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="324d1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="324d1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="324d1-121">Request headers</span></span>

| <span data-ttu-id="324d1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="324d1-122">Name</span></span>      |<span data-ttu-id="324d1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="324d1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="324d1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="324d1-124">Authorization</span></span> | <span data-ttu-id="324d1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="324d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="324d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="324d1-127">Request body</span></span>

<span data-ttu-id="324d1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="324d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="324d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="324d1-129">Response</span></span>

<span data-ttu-id="324d1-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="324d1-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="324d1-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="324d1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="324d1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="324d1-132">Request</span></span>

<span data-ttu-id="324d1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="324d1-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="324d1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="324d1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="324d1-135">C#</span><span class="sxs-lookup"><span data-stu-id="324d1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="324d1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="324d1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="324d1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="324d1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="324d1-138">Java</span><span class="sxs-lookup"><span data-stu-id="324d1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="324d1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="324d1-139">Response</span></span>

<span data-ttu-id="324d1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="324d1-140">The following is an example of the response.</span></span>

> <span data-ttu-id="324d1-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="324d1-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
