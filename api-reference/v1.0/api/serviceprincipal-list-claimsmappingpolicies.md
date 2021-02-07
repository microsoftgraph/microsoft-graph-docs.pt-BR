---
title: Listar claimsMappingPolicies atribuída
description: Listar claimsMappingPolicies que são atribuídas a uma entidade de serviço.
localization_priority: Normal
author: paulgarn
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8282d90d6df5c44432a203c46438317bd9f15515
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132234"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="ea217-103">Listar claimsMappingPolicy atribuída</span><span class="sxs-lookup"><span data-stu-id="ea217-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="ea217-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea217-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ea217-105">Listar [os objetos claimsMappingPolicy](../resources/claimsmappingpolicy.md) que são atribuídos a [um servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="ea217-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea217-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ea217-106">Permissions</span></span>

<span data-ttu-id="ea217-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea217-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea217-109">Permission type</span></span>                        | <span data-ttu-id="ea217-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea217-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea217-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea217-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea217-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea217-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ea217-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea217-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea217-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea217-114">Not supported.</span></span> |
| <span data-ttu-id="ea217-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea217-115">Application</span></span>                            | <span data-ttu-id="ea217-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea217-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea217-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea217-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ea217-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea217-118">Request headers</span></span>

| <span data-ttu-id="ea217-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ea217-119">Name</span></span>          | <span data-ttu-id="ea217-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea217-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ea217-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea217-121">Authorization</span></span> | <span data-ttu-id="ea217-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea217-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea217-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea217-124">Request body</span></span>

<span data-ttu-id="ea217-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea217-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea217-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea217-126">Response</span></span>

<span data-ttu-id="ea217-127">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea217-127">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea217-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ea217-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea217-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea217-129">Request</span></span>

<span data-ttu-id="ea217-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea217-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea217-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea217-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="ea217-132">C#</span><span class="sxs-lookup"><span data-stu-id="ea217-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea217-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea217-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea217-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea217-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea217-135">Java</span><span class="sxs-lookup"><span data-stu-id="ea217-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-claimsmappingpolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea217-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea217-136">Response</span></span>

<span data-ttu-id="ea217-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea217-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ea217-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea217-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
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
  "description": "List assigned claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

