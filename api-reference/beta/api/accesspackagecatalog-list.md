---
title: Listar accessPackageCatalogs
description: Recupere uma lista de objetos accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 729d7504fc7cfffcb80f763f7b6c428e90b4bf31
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345426"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="1be24-103">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="1be24-103">List accessPackageCatalogs</span></span>

<span data-ttu-id="1be24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be24-105">Recupere uma lista de objetos [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="1be24-105">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1be24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1be24-106">Permissions</span></span>

<span data-ttu-id="1be24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1be24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1be24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1be24-109">Permission type</span></span>                        | <span data-ttu-id="1be24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1be24-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1be24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1be24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1be24-112">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1be24-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1be24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1be24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1be24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be24-114">Not supported.</span></span> |
| <span data-ttu-id="1be24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1be24-115">Application</span></span>                            | <span data-ttu-id="1be24-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1be24-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1be24-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1be24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1be24-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1be24-118">Optional query parameters</span></span>

<span data-ttu-id="1be24-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1be24-119">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="1be24-120">Por exemplo, para recuperar os pacotes de acesso em cada catálogo, inclua `$expand=accessPackages` a consulta.</span><span class="sxs-lookup"><span data-stu-id="1be24-120">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="1be24-121">Para pesquisar catálogos de pacotes do Access com um nome específico, inclua um filtro como `$filter=contains(tolower(displayName),'staff')` na consulta.</span><span class="sxs-lookup"><span data-stu-id="1be24-121">To search for access package catalogs with a particular name, include a filter such as `$filter=contains(tolower(displayName),'staff')` in the query.</span></span>  <span data-ttu-id="1be24-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1be24-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1be24-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1be24-123">Request headers</span></span>

| <span data-ttu-id="1be24-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1be24-124">Name</span></span>      |<span data-ttu-id="1be24-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be24-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1be24-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1be24-126">Authorization</span></span> | <span data-ttu-id="1be24-127">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1be24-127">Bearer \{token\}.</span></span> <span data-ttu-id="1be24-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be24-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1be24-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1be24-129">Request body</span></span>

<span data-ttu-id="1be24-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1be24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1be24-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be24-131">Response</span></span>

<span data-ttu-id="1be24-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1be24-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1be24-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1be24-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1be24-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1be24-134">Request</span></span>

<span data-ttu-id="1be24-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1be24-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1be24-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1be24-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="c"></a>[<span data-ttu-id="1be24-137">C#</span><span class="sxs-lookup"><span data-stu-id="1be24-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1be24-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1be24-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1be24-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1be24-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1be24-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1be24-140">Response</span></span>

<span data-ttu-id="1be24-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1be24-141">The following is an example of the response.</span></span>

> <span data-ttu-id="1be24-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1be24-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
