---
title: Listar accessPackages
description: Recupere uma lista de objetos accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1b4a364c980feeb311e64f67bec50993e51a742c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038562"
---
# <a name="list-accesspackages"></a><span data-ttu-id="1af0b-103">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="1af0b-103">List accessPackages</span></span>

<span data-ttu-id="1af0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1af0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af0b-105">Recupere uma lista de [objetos accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="1af0b-105">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="1af0b-106">A lista resultante inclui todos os pacotes de acesso que o chamador tem acesso para ler, em todos os catálogos.</span><span class="sxs-lookup"><span data-stu-id="1af0b-106">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="1af0b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1af0b-107">Permissions</span></span>

<span data-ttu-id="1af0b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1af0b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1af0b-110">Permission type</span></span>                        | <span data-ttu-id="1af0b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1af0b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1af0b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1af0b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1af0b-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1af0b-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1af0b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1af0b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1af0b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1af0b-115">Not supported.</span></span> |
| <span data-ttu-id="1af0b-116">Application</span><span class="sxs-lookup"><span data-stu-id="1af0b-116">Application</span></span>                            | <span data-ttu-id="1af0b-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1af0b-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1af0b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1af0b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1af0b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1af0b-119">Optional query parameters</span></span>

<span data-ttu-id="1af0b-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1af0b-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1af0b-121">Por exemplo, para recuperar as políticas de pacote de acesso para cada pacote de acesso, adicione `$expand=accessPackageAssignmentPolicies` .</span><span class="sxs-lookup"><span data-stu-id="1af0b-121">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="1af0b-122">Para pesquisar pacotes de acesso com um nome específico, inclua um filtro como `$filter=contains(tolower(displayName),'team')` na consulta.</span><span class="sxs-lookup"><span data-stu-id="1af0b-122">To search for access packages with a particular name, include a filter such as `$filter=contains(tolower(displayName),'team')` in the query.</span></span> <span data-ttu-id="1af0b-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1af0b-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1af0b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1af0b-124">Request headers</span></span>

| <span data-ttu-id="1af0b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1af0b-125">Name</span></span>      |<span data-ttu-id="1af0b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1af0b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1af0b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1af0b-127">Authorization</span></span> | <span data-ttu-id="1af0b-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1af0b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1af0b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1af0b-130">Request body</span></span>

<span data-ttu-id="1af0b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1af0b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1af0b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1af0b-132">Response</span></span>

<span data-ttu-id="1af0b-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1af0b-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1af0b-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1af0b-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1af0b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1af0b-135">Request</span></span>

<span data-ttu-id="1af0b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1af0b-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1af0b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1af0b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="c"></a>[<span data-ttu-id="1af0b-138">C#</span><span class="sxs-lookup"><span data-stu-id="1af0b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1af0b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1af0b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1af0b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1af0b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1af0b-141">Java</span><span class="sxs-lookup"><span data-stu-id="1af0b-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1af0b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1af0b-142">Response</span></span>

<span data-ttu-id="1af0b-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1af0b-143">The following is an example of the response.</span></span>

> <span data-ttu-id="1af0b-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1af0b-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package",
      "displayName":"Access package for testing",
      "isHidden":false,
      "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
      "isRoleScopesVisible":false,
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


