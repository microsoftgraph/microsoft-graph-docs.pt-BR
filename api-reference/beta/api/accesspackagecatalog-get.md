---
title: Obter accessPackageCatalog
description: Recupere as propriedades e as relações do objeto accesspackagecatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b80f81eb09fbebc539a9fd5e523f0f4b9daf7c4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048572"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="3cbc5-103">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3cbc5-103">Get accessPackageCatalog</span></span>

<span data-ttu-id="3cbc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cbc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cbc5-105">Recupere as propriedades e as relações de um [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="3cbc5-105">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cbc5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cbc5-106">Permissions</span></span>

<span data-ttu-id="3cbc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cbc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3cbc5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cbc5-109">Permission type</span></span>                        | <span data-ttu-id="3cbc5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cbc5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3cbc5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cbc5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cbc5-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cbc5-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3cbc5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cbc5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cbc5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-114">Not supported.</span></span> |
| <span data-ttu-id="3cbc5-115">Application</span><span class="sxs-lookup"><span data-stu-id="3cbc5-115">Application</span></span>                            | <span data-ttu-id="3cbc5-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cbc5-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cbc5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cbc5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cbc5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3cbc5-118">Optional query parameters</span></span>

<span data-ttu-id="3cbc5-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3cbc5-120">Por exemplo, para recuperar os pacotes de acesso em um catálogo, `$expand=accessPackages` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-120">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="3cbc5-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3cbc5-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cbc5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cbc5-122">Request headers</span></span>

| <span data-ttu-id="3cbc5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3cbc5-123">Name</span></span>      |<span data-ttu-id="3cbc5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cbc5-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3cbc5-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cbc5-125">Authorization</span></span> | <span data-ttu-id="3cbc5-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cbc5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cbc5-128">Request body</span></span>

<span data-ttu-id="3cbc5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cbc5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cbc5-130">Response</span></span>

<span data-ttu-id="3cbc5-131">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cbc5-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3cbc5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cbc5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cbc5-133">Request</span></span>

<span data-ttu-id="3cbc5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cbc5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cbc5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="3cbc5-136">C#</span><span class="sxs-lookup"><span data-stu-id="3cbc5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cbc5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cbc5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cbc5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cbc5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cbc5-139">Java</span><span class="sxs-lookup"><span data-stu-id="3cbc5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3cbc5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cbc5-140">Response</span></span>

<span data-ttu-id="3cbc5-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-141">The following is an example of the response.</span></span>

> <span data-ttu-id="3cbc5-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3cbc5-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


