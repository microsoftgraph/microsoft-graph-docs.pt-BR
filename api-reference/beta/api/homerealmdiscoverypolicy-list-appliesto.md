---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 31ea1eb539dc22dce69c3330d641c67188318067
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040970"
---
# <a name="list-appliesto"></a><span data-ttu-id="37145-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="37145-103">List appliesTo</span></span>

<span data-ttu-id="37145-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37145-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37145-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual um [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="37145-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="37145-106">O homeRealmDiscoveryPolicy só pode ser aplicado aos [recursos servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="37145-106">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="37145-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="37145-107">Permissions</span></span>

<span data-ttu-id="37145-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37145-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37145-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37145-110">Permission type</span></span>                        | <span data-ttu-id="37145-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37145-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37145-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37145-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="37145-113">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="37145-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="37145-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37145-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37145-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37145-115">Not supported.</span></span> |
| <span data-ttu-id="37145-116">Application</span><span class="sxs-lookup"><span data-stu-id="37145-116">Application</span></span>                            | <span data-ttu-id="37145-117">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="37145-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37145-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37145-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37145-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37145-119">Optional query parameters</span></span>

<span data-ttu-id="37145-120">Este método dá suporte aos `$select` `$top` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37145-120">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="37145-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37145-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37145-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37145-122">Request headers</span></span>

| <span data-ttu-id="37145-123">Nome</span><span class="sxs-lookup"><span data-stu-id="37145-123">Name</span></span>      |<span data-ttu-id="37145-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="37145-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37145-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="37145-125">Authorization</span></span> | <span data-ttu-id="37145-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="37145-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="37145-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37145-127">Request body</span></span>

<span data-ttu-id="37145-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37145-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37145-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37145-129">Response</span></span>

<span data-ttu-id="37145-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37145-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37145-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37145-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37145-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37145-132">Request</span></span>

<span data-ttu-id="37145-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37145-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37145-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="37145-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="37145-135">C#</span><span class="sxs-lookup"><span data-stu-id="37145-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37145-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37145-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37145-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37145-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37145-138">Java</span><span class="sxs-lookup"><span data-stu-id="37145-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37145-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="37145-139">Response</span></span>

<span data-ttu-id="37145-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37145-140">The following is an example of the response.</span></span>

> <span data-ttu-id="37145-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37145-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

