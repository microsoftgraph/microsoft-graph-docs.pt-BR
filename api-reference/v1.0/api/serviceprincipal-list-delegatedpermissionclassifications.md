---
title: Listar a coleção delegatedPermissionClassifications de servicePrincipal
description: Recupere uma lista de classificações dadas a permissões delegadas expostas pela entidade de serviço de uma API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4ab551d0e8d23a2d8810d3bc10c812318aaaaa10
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132227"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="c8e82-103">Listar a coleção delegatedPermissionClassifications de servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c8e82-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="c8e82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c8e82-105">Recupere a lista [de delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) atualmente configurada para as permissões delegadas expostas por uma API.</span><span class="sxs-lookup"><span data-stu-id="c8e82-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e82-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8e82-106">Permissions</span></span>

<span data-ttu-id="c8e82-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e82-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8e82-109">Permission type</span></span>      | <span data-ttu-id="c8e82-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8e82-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8e82-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8e82-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8e82-112">Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e82-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="c8e82-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8e82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e82-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8e82-114">Not supported.</span></span>    |
|<span data-ttu-id="c8e82-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8e82-115">Application</span></span> | <span data-ttu-id="c8e82-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e82-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8e82-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8e82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e82-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c8e82-118">Optional query parameters</span></span>

<span data-ttu-id="c8e82-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c8e82-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e82-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8e82-120">Request headers</span></span>

| <span data-ttu-id="c8e82-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c8e82-121">Name</span></span>           | <span data-ttu-id="c8e82-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8e82-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c8e82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8e82-123">Authorization</span></span>  | <span data-ttu-id="c8e82-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8e82-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8e82-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8e82-126">Request body</span></span>

<span data-ttu-id="c8e82-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8e82-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e82-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8e82-128">Response</span></span>

<span data-ttu-id="c8e82-129">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8e82-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e82-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8e82-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8e82-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8e82-131">Request</span></span>

<span data-ttu-id="c8e82-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8e82-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8e82-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8e82-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
```
# <a name="c"></a>[<span data-ttu-id="c8e82-134">C#</span><span class="sxs-lookup"><span data-stu-id="c8e82-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8e82-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8e82-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8e82-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8e82-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8e82-137">Java</span><span class="sxs-lookup"><span data-stu-id="c8e82-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8e82-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8e82-138">Response</span></span>

<span data-ttu-id="c8e82-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8e82-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c8e82-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8e82-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id": "2G3-4TG6YU2J54hjnaRoPQE",
        "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
        "permissionName": "User.Read",
        "classification": "low"
    }
  ]
}
```
