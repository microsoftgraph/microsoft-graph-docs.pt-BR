---
title: Obter accessPackageCatalog
description: Recupere as propriedades e os relacionamentos do objeto accesspackagecatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b13becb36bbcc9fb4eb579f1997c66ae7262fe2b
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345473"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="ce0c4-103">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="ce0c4-103">Get accessPackageCatalog</span></span>

<span data-ttu-id="ce0c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce0c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce0c4-105">Recupere as propriedades e os relacionamentos de um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="ce0c4-105">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce0c4-106">Permissions</span></span>

<span data-ttu-id="ce0c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce0c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce0c4-109">Permission type</span></span>                        | <span data-ttu-id="ce0c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce0c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce0c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce0c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce0c4-112">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ce0c4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ce0c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce0c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce0c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-114">Not supported.</span></span> |
| <span data-ttu-id="ce0c4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce0c4-115">Application</span></span>                            | <span data-ttu-id="ce0c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce0c4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce0c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce0c4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce0c4-118">Optional query parameters</span></span>

<span data-ttu-id="ce0c4-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce0c4-120">Por exemplo, para recuperar os pacotes do Access em um catálogo, inclua `$expand=accessPackages` a consulta.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-120">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="ce0c4-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ce0c4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce0c4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c4-122">Request headers</span></span>

| <span data-ttu-id="ce0c4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ce0c4-123">Name</span></span>      |<span data-ttu-id="ce0c4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce0c4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce0c4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce0c4-125">Authorization</span></span> | <span data-ttu-id="ce0c4-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-126">Bearer \{token\}.</span></span> <span data-ttu-id="ce0c4-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce0c4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c4-128">Request body</span></span>

<span data-ttu-id="ce0c4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce0c4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c4-130">Response</span></span>

<span data-ttu-id="ce0c4-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce0c4-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce0c4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce0c4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c4-133">Request</span></span>

<span data-ttu-id="ce0c4-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce0c4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce0c4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="ce0c4-136">C#</span><span class="sxs-lookup"><span data-stu-id="ce0c4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce0c4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce0c4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce0c4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce0c4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce0c4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c4-139">Response</span></span>

<span data-ttu-id="ce0c4-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-140">The following is an example of the response.</span></span>

> <span data-ttu-id="ce0c4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce0c4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
