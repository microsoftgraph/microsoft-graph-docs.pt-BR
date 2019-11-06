---
title: Listar accessPackageCatalogs
description: Recupere uma lista de objetos accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1d8aaf8a0138195e737cdd26f288f7aca8ba3e5
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994236"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="9e812-103">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="9e812-103">List accessPackageCatalogs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e812-104">Recupere uma lista de objetos [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="9e812-104">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e812-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e812-105">Permissions</span></span>

<span data-ttu-id="9e812-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e812-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e812-108">Permission type</span></span>                        | <span data-ttu-id="9e812-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e812-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e812-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e812-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="9e812-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e812-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9e812-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e812-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e812-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e812-113">Not supported.</span></span> |
| <span data-ttu-id="9e812-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e812-114">Application</span></span>                            | <span data-ttu-id="9e812-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e812-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e812-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e812-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e812-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e812-117">Optional query parameters</span></span>

<span data-ttu-id="9e812-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e812-118">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="9e812-119">Por exemplo, para recuperar os pacotes de acesso em cada catálogo, `$expand=accessPackages` inclua a consulta.</span><span class="sxs-lookup"><span data-stu-id="9e812-119">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="9e812-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9e812-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e812-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e812-121">Request headers</span></span>

| <span data-ttu-id="9e812-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9e812-122">Name</span></span>      |<span data-ttu-id="9e812-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e812-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e812-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e812-124">Authorization</span></span> | <span data-ttu-id="9e812-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="9e812-125">Bearer \{token\}.</span></span> <span data-ttu-id="9e812-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e812-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e812-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e812-127">Request body</span></span>

<span data-ttu-id="9e812-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e812-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e812-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e812-129">Response</span></span>

<span data-ttu-id="9e812-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageCatalog](../resources/accesspackagecatalog.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e812-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e812-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e812-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e812-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e812-132">Request</span></span>

<span data-ttu-id="9e812-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e812-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9e812-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e812-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9e812-135">C#</span><span class="sxs-lookup"><span data-stu-id="9e812-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9e812-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e812-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9e812-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e812-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e812-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e812-138">Response</span></span>

<span data-ttu-id="9e812-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e812-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9e812-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e812-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
