---
title: Obter identitySecurityDefaultsEnforcementPolicy
description: Recupere as propriedades e os relacionamentos do objeto identitysecuritydefaultsenforcementpolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9eb969ab7a8125e91acee1a3e0528851164bbe16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033402"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="62ecb-103">Obter identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="62ecb-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="62ecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62ecb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62ecb-105">Recupere as propriedades de um objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="62ecb-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62ecb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="62ecb-106">Permissions</span></span>

<span data-ttu-id="62ecb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62ecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62ecb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62ecb-109">Permission type</span></span>                        | <span data-ttu-id="62ecb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62ecb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62ecb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62ecb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62ecb-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="62ecb-112">Policy.Read.All</span></span> |
| <span data-ttu-id="62ecb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62ecb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62ecb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62ecb-114">Not supported.</span></span> |
| <span data-ttu-id="62ecb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62ecb-115">Application</span></span>                            | <span data-ttu-id="62ecb-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="62ecb-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62ecb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62ecb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62ecb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62ecb-118">Optional query parameters</span></span>

<span data-ttu-id="62ecb-119">Este método oferece suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62ecb-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="62ecb-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="62ecb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62ecb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62ecb-121">Request headers</span></span>

| <span data-ttu-id="62ecb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="62ecb-122">Name</span></span>      |<span data-ttu-id="62ecb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="62ecb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62ecb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62ecb-124">Authorization</span></span> | <span data-ttu-id="62ecb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62ecb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62ecb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62ecb-127">Request body</span></span>

<span data-ttu-id="62ecb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62ecb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62ecb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62ecb-129">Response</span></span>

<span data-ttu-id="62ecb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62ecb-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62ecb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62ecb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62ecb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62ecb-132">Request</span></span>

<span data-ttu-id="62ecb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62ecb-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62ecb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="62ecb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="62ecb-135">C#</span><span class="sxs-lookup"><span data-stu-id="62ecb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62ecb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62ecb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62ecb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62ecb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62ecb-138">Java</span><span class="sxs-lookup"><span data-stu-id="62ecb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62ecb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="62ecb-139">Response</span></span>

<span data-ttu-id="62ecb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62ecb-140">The following is an example of the response.</span></span>

> <span data-ttu-id="62ecb-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62ecb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

