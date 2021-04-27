---
title: Listar tokens atribuídosIssuancePolicies
description: Listar tokenIssuancePolicies atribuídas a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: be0d2e7e113d676c97d03e45262d901a3482ba1a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048110"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="3d6f3-103">Listar tokens atribuídosIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="3d6f3-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="3d6f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d6f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d6f3-105">Listar [os objetos tokenIssuancePolicy](../resources/tokenissuancepolicy.md) atribuídos a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="3d6f3-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d6f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d6f3-106">Permissions</span></span>

<span data-ttu-id="3d6f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d6f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d6f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d6f3-109">Permission type</span></span>                        | <span data-ttu-id="3d6f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d6f3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d6f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d6f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d6f3-112">Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d6f3-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="3d6f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d6f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d6f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-114">Not supported.</span></span> |
| <span data-ttu-id="3d6f3-115">Application</span><span class="sxs-lookup"><span data-stu-id="3d6f3-115">Application</span></span>                            | <span data-ttu-id="3d6f3-116">Policy.Read.All e Application.ReadWrite.OwnedBy, Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d6f3-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d6f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d6f3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3d6f3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d6f3-118">Request headers</span></span>

| <span data-ttu-id="3d6f3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3d6f3-119">Name</span></span>          | <span data-ttu-id="3d6f3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d6f3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3d6f3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d6f3-121">Authorization</span></span> | <span data-ttu-id="3d6f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d6f3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d6f3-124">Request body</span></span>

<span data-ttu-id="3d6f3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d6f3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d6f3-126">Response</span></span>

<span data-ttu-id="3d6f3-127">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d6f3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d6f3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d6f3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d6f3-129">Request</span></span>

<span data-ttu-id="3d6f3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d6f3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d6f3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="3d6f3-132">C#</span><span class="sxs-lookup"><span data-stu-id="3d6f3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d6f3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d6f3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d6f3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d6f3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d6f3-135">Java</span><span class="sxs-lookup"><span data-stu-id="3d6f3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenissuancepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3d6f3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d6f3-136">Response</span></span>

<span data-ttu-id="3d6f3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="3d6f3-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d6f3-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
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
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



