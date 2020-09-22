---
title: Lista atribuída tokenIssuancePolicies
description: Listar tokenIssuancePolicies atribuídos a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bbc1f7254088887fd295abb8348e7818e33f85e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996896"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="2f2e0-103">Lista atribuída tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="2f2e0-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="2f2e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f2e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f2e0-105">Lista os objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="2f2e0-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f2e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f2e0-106">Permissions</span></span>

<span data-ttu-id="2f2e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f2e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f2e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f2e0-109">Permission type</span></span>                        | <span data-ttu-id="2f2e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f2e0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f2e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f2e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f2e0-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2f2e0-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="2f2e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f2e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f2e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-114">Not supported.</span></span> |
| <span data-ttu-id="2f2e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f2e0-115">Application</span></span>                            | <span data-ttu-id="2f2e0-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2f2e0-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f2e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f2e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2f2e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2e0-118">Request headers</span></span>

| <span data-ttu-id="2f2e0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2f2e0-119">Name</span></span>          | <span data-ttu-id="2f2e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f2e0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2f2e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f2e0-121">Authorization</span></span> | <span data-ttu-id="2f2e0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f2e0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2e0-124">Request body</span></span>

<span data-ttu-id="2f2e0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f2e0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2e0-126">Response</span></span>

<span data-ttu-id="2f2e0-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f2e0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2f2e0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f2e0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f2e0-129">Request</span></span>

<span data-ttu-id="2f2e0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f2e0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f2e0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="2f2e0-132">C#</span><span class="sxs-lookup"><span data-stu-id="2f2e0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f2e0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f2e0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f2e0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f2e0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f2e0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f2e0-135">Response</span></span>

<span data-ttu-id="2f2e0-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-136">The following is an example of the response.</span></span>

> <span data-ttu-id="2f2e0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f2e0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


