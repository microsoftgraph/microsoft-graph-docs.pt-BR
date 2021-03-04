---
title: Listar accessPackageResourceRoles
description: Recupere uma lista de objetos accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9d3a8c243b6e2789fada38dec2643f3cd9bd1bd9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439560"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="45fda-103">Listar accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="45fda-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="45fda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45fda-105">Recupere uma lista de [objetos accessPackageResourceRole](../resources/accesspackageresourcerole.md) de [um accessPackageResource](../resources/accesspackageresource.md) em [um accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="45fda-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="45fda-106">Essa lista de funções pode ser usada pelo chamador para selecionar uma função, que é necessária ao criar posteriormente um [accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="45fda-106">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45fda-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="45fda-107">Permissions</span></span>

<span data-ttu-id="45fda-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45fda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45fda-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45fda-110">Permission type</span></span>                        | <span data-ttu-id="45fda-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45fda-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="45fda-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45fda-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="45fda-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45fda-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="45fda-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45fda-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45fda-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45fda-115">Not supported.</span></span> |
| <span data-ttu-id="45fda-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45fda-116">Application</span></span>                            | <span data-ttu-id="45fda-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45fda-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45fda-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45fda-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45fda-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45fda-119">Optional query parameters</span></span>

<span data-ttu-id="45fda-120">Este método usa parâmetros de consulta OData para construir a resposta.</span><span class="sxs-lookup"><span data-stu-id="45fda-120">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="45fda-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45fda-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45fda-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45fda-122">Request headers</span></span>

| <span data-ttu-id="45fda-123">Nome</span><span class="sxs-lookup"><span data-stu-id="45fda-123">Name</span></span>      |<span data-ttu-id="45fda-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="45fda-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="45fda-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="45fda-125">Authorization</span></span> | <span data-ttu-id="45fda-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45fda-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45fda-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45fda-128">Request body</span></span>

<span data-ttu-id="45fda-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45fda-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45fda-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="45fda-130">Response</span></span>

<span data-ttu-id="45fda-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceRole](../resources/accesspackageresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45fda-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45fda-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45fda-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45fda-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45fda-133">Request</span></span>

<span data-ttu-id="45fda-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="45fda-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45fda-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="45fda-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="45fda-136">C#</span><span class="sxs-lookup"><span data-stu-id="45fda-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45fda-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45fda-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45fda-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45fda-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45fda-139">Java</span><span class="sxs-lookup"><span data-stu-id="45fda-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45fda-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="45fda-140">Response</span></span>

<span data-ttu-id="45fda-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="45fda-141">The following is an example of the response.</span></span>

> <span data-ttu-id="45fda-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45fda-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


