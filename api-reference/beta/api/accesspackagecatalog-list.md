---
title: Listar accessPackageCatalogs
description: Recupere uma lista de objetos accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c4f4d959792e657f79d0242a52944da505a41695
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439545"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="8cc0b-103">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="8cc0b-103">List accessPackageCatalogs</span></span>

<span data-ttu-id="8cc0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc0b-105">Recupere uma lista de [objetos accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="8cc0b-105">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cc0b-106">Permissions</span></span>

<span data-ttu-id="8cc0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cc0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc0b-109">Permission type</span></span>                        | <span data-ttu-id="8cc0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cc0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cc0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cc0b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc0b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8cc0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-114">Not supported.</span></span> |
| <span data-ttu-id="8cc0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc0b-115">Application</span></span>                            | <span data-ttu-id="8cc0b-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc0b-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cc0b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8cc0b-118">Optional query parameters</span></span>

<span data-ttu-id="8cc0b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-119">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="8cc0b-120">Por exemplo, para recuperar os pacotes de acesso em cada catálogo, `$expand=accessPackages` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-120">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="8cc0b-121">Para pesquisar catálogos de pacotes de acesso com um nome específico, inclua um filtro como `$filter=contains(tolower(displayName),'staff')` na consulta.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-121">To search for access package catalogs with a particular name, include a filter such as `$filter=contains(tolower(displayName),'staff')` in the query.</span></span>  <span data-ttu-id="8cc0b-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8cc0b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cc0b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc0b-123">Request headers</span></span>

| <span data-ttu-id="8cc0b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8cc0b-124">Name</span></span>      |<span data-ttu-id="8cc0b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc0b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cc0b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc0b-126">Authorization</span></span> | <span data-ttu-id="8cc0b-127">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-127">Bearer \{token\}.</span></span> <span data-ttu-id="8cc0b-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc0b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc0b-129">Request body</span></span>

<span data-ttu-id="8cc0b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cc0b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc0b-131">Response</span></span>

<span data-ttu-id="8cc0b-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cc0b-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8cc0b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cc0b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc0b-134">Request</span></span>

<span data-ttu-id="8cc0b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cc0b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc0b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="c"></a>[<span data-ttu-id="8cc0b-137">C#</span><span class="sxs-lookup"><span data-stu-id="8cc0b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cc0b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc0b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cc0b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc0b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cc0b-140">Java</span><span class="sxs-lookup"><span data-stu-id="8cc0b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cc0b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc0b-141">Response</span></span>

<span data-ttu-id="8cc0b-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-142">The following is an example of the response.</span></span>

> <span data-ttu-id="8cc0b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc0b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package catalog",
      "displayName":"Access package catalog for testing",
      "isExternallyVisible":false,
      "catalogType":"UserManaged",
      "catalogStatus":"Published",
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
  "description": "List accessPackageCatalogs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


