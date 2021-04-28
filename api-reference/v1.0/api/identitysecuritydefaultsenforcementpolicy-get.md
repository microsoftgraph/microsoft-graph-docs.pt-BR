---
title: Obter identitySecurityDefaultsEnforcementPolicy
description: Recupere as propriedades e as relações do objeto identitysecuritydefaultsenforcementpolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8d4f85522374444183d06fd0715bc24ba937d678
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051379"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="17c9e-103">Obter identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="17c9e-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="17c9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17c9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17c9e-105">Recupere as propriedades de [um objeto identitySecurityDefaultsEnforcementPolicy.](../resources/identitysecuritydefaultsenforcementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="17c9e-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17c9e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17c9e-106">Permissions</span></span>

<span data-ttu-id="17c9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17c9e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17c9e-109">Permission type</span></span>                        | <span data-ttu-id="17c9e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17c9e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="17c9e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17c9e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17c9e-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="17c9e-112">Policy.Read.All</span></span> |
| <span data-ttu-id="17c9e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17c9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17c9e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17c9e-114">Not supported.</span></span> |
| <span data-ttu-id="17c9e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c9e-115">Application</span></span>                            | <span data-ttu-id="17c9e-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="17c9e-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17c9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17c9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17c9e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17c9e-118">Optional query parameters</span></span>

<span data-ttu-id="17c9e-119">Este método dá suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17c9e-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="17c9e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="17c9e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17c9e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17c9e-121">Request headers</span></span>

| <span data-ttu-id="17c9e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="17c9e-122">Name</span></span>      |<span data-ttu-id="17c9e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c9e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17c9e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17c9e-124">Authorization</span></span> | <span data-ttu-id="17c9e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c9e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17c9e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17c9e-127">Request body</span></span>

<span data-ttu-id="17c9e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17c9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17c9e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c9e-129">Response</span></span>

<span data-ttu-id="17c9e-130">Se tiver êxito, este método retornará um código de resposta e o `200 OK` objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17c9e-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17c9e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17c9e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17c9e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17c9e-132">Request</span></span>

<span data-ttu-id="17c9e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17c9e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="17c9e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="17c9e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="17c9e-135">C#</span><span class="sxs-lookup"><span data-stu-id="17c9e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17c9e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17c9e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17c9e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17c9e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17c9e-138">Java</span><span class="sxs-lookup"><span data-stu-id="17c9e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17c9e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c9e-139">Response</span></span>

<span data-ttu-id="17c9e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17c9e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="17c9e-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="17c9e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

