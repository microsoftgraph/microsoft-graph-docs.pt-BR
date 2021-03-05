---
title: Obter identitySecurityDefaultsEnforcementPolicy
description: Recupere as propriedades e as relações do objeto identitysecuritydefaultsenforcementpolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 927de49830838e219b164eaac1be4fbcd7d657e9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441822"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="90f38-103">Obter identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="90f38-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="90f38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90f38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90f38-105">Recupere as propriedades de [um objeto identitySecurityDefaultsEnforcementPolicy.](../resources/identitysecuritydefaultsenforcementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90f38-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90f38-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="90f38-106">Permissions</span></span>

<span data-ttu-id="90f38-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90f38-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90f38-109">Permission type</span></span>                        | <span data-ttu-id="90f38-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90f38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90f38-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90f38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90f38-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="90f38-112">Policy.Read.All</span></span> |
| <span data-ttu-id="90f38-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90f38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90f38-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90f38-114">Not supported.</span></span> |
| <span data-ttu-id="90f38-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90f38-115">Application</span></span>                            | <span data-ttu-id="90f38-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="90f38-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90f38-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90f38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90f38-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90f38-118">Optional query parameters</span></span>

<span data-ttu-id="90f38-119">Este método dá suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90f38-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="90f38-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="90f38-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90f38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90f38-121">Request headers</span></span>

| <span data-ttu-id="90f38-122">Nome</span><span class="sxs-lookup"><span data-stu-id="90f38-122">Name</span></span>      |<span data-ttu-id="90f38-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="90f38-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90f38-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="90f38-124">Authorization</span></span> | <span data-ttu-id="90f38-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90f38-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90f38-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90f38-127">Request body</span></span>

<span data-ttu-id="90f38-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90f38-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90f38-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f38-129">Response</span></span>

<span data-ttu-id="90f38-130">Se tiver êxito, este método retornará um código de resposta e o `200 OK` objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90f38-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90f38-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="90f38-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90f38-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90f38-132">Request</span></span>

<span data-ttu-id="90f38-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="90f38-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="90f38-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="90f38-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="90f38-135">C#</span><span class="sxs-lookup"><span data-stu-id="90f38-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90f38-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90f38-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90f38-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90f38-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90f38-138">Java</span><span class="sxs-lookup"><span data-stu-id="90f38-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90f38-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="90f38-139">Response</span></span>

<span data-ttu-id="90f38-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="90f38-140">The following is an example of the response.</span></span>

> <span data-ttu-id="90f38-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90f38-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

