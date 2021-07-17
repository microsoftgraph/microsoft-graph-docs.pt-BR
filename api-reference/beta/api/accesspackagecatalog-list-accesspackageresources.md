---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3aaeddef635a80bb8a54d3680281b8b9edae98ae
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466940"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="ddb1d-103">Listar accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="ddb1d-103">List accessPackageResources</span></span>

<span data-ttu-id="ddb1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb1d-105">Recuperar uma lista de [objetos accessPackageResource](../resources/accesspackageresource.md) em [um accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="ddb1d-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="ddb1d-106">Para solicitar para adicionar ou remover [um accessPackageResource,](../resources/accesspackageresource.md)use [criar accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="ddb1d-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddb1d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddb1d-107">Permissions</span></span>

<span data-ttu-id="ddb1d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddb1d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddb1d-110">Permission type</span></span>                        | <span data-ttu-id="ddb1d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddb1d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddb1d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddb1d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddb1d-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb1d-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ddb1d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddb1d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-115">Not supported.</span></span> |
| <span data-ttu-id="ddb1d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddb1d-116">Application</span></span>                            | <span data-ttu-id="ddb1d-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb1d-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb1d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb1d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ddb1d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ddb1d-119">Optional query parameters</span></span>

<span data-ttu-id="ddb1d-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="ddb1d-121">Por exemplo, para recuperar os escopos e ambientes de recursos do pacote de acesso para cada recurso, `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-121">For example, to retrieve the access package resource scopes and environments for each resource, include `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span> <span data-ttu-id="ddb1d-122">Para recuperar as funções disponíveis de um recurso, inclua `$expand=accessPackageResourceRoles` .</span><span class="sxs-lookup"><span data-stu-id="ddb1d-122">To retrieve the available roles of a resource, include `$expand=accessPackageResourceRoles`.</span></span> <span data-ttu-id="ddb1d-123">Para recuperar apenas recursos para aplicativos e não grupos ou sites, `$filter=resourceType eq 'Application'` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-123">To retrieve only resources for applications and not groups or sites, include `$filter=resourceType eq 'Application'` in the query.</span></span> <span data-ttu-id="ddb1d-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ddb1d-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddb1d-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb1d-125">Request headers</span></span>

| <span data-ttu-id="ddb1d-126">Nome</span><span class="sxs-lookup"><span data-stu-id="ddb1d-126">Name</span></span>      |<span data-ttu-id="ddb1d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb1d-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddb1d-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddb1d-128">Authorization</span></span> | <span data-ttu-id="ddb1d-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddb1d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb1d-131">Request body</span></span>

<span data-ttu-id="ddb1d-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddb1d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb1d-133">Response</span></span>

<span data-ttu-id="ddb1d-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddb1d-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddb1d-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddb1d-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb1d-136">Request</span></span>

<span data-ttu-id="ddb1d-137">A seguir está um exemplo da solicitação, usando um filtro para selecionar recursos de um tipo específico e para retornar escopos de `$expand` recurso de cada recurso.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-137">The following is an example of the request, using a filter to select resources of a particular type and `$expand` to return resource scopes of each resource.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddb1d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb1d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[<span data-ttu-id="ddb1d-139">C#</span><span class="sxs-lookup"><span data-stu-id="ddb1d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddb1d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb1d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddb1d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddb1d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddb1d-142">Java</span><span class="sxs-lookup"><span data-stu-id="ddb1d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ddb1d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb1d-143">Response</span></span>

<span data-ttu-id="ddb1d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-144">The following is an example of the response.</span></span>

> <span data-ttu-id="ddb1d-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ddb1d-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
         {
            "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
            "displayName": "Root",
            "description": "Root Scope",
            "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
            "originSystem": "AadApplication",
            "isRootScope": true
         }
      ]
    }
  ]
}
```

https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/e71fafe7-9ccb-4c5a-a7b3-77ec35e83e3c/accessPackageResources

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


