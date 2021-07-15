---
title: Listar accessPackageResourceRoles
description: Recupere uma lista de objetos accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 45e8f2364997518bbc47d61906a9e3f4986e64e6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439249"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="a1079-103">Listar accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="a1079-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="a1079-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1079-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1079-105">Recupere uma lista de [objetos accessPackageResourceRole](../resources/accesspackageresourcerole.md) de [um accessPackageResource](../resources/accesspackageresource.md) em [um accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="a1079-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="a1079-106">O recurso deve ter sido adicionado ao catálogo criando [um accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="a1079-106">The resource should have been added to the catalog by [creating an accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span> <span data-ttu-id="a1079-107">Essa lista de funções pode ser usada pelo chamador para selecionar uma função, que é necessária ao criar posteriormente um [accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="a1079-107">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1079-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a1079-108">Permissions</span></span>

<span data-ttu-id="a1079-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1079-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1079-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1079-111">Permission type</span></span>                        | <span data-ttu-id="a1079-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1079-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1079-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1079-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1079-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1079-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a1079-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1079-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1079-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1079-116">Not supported.</span></span> |
| <span data-ttu-id="a1079-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1079-117">Application</span></span>                            | <span data-ttu-id="a1079-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1079-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1079-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1079-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1079-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1079-120">Optional query parameters</span></span>

<span data-ttu-id="a1079-121">Este método usa parâmetros de consulta OData para construir a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1079-121">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="a1079-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a1079-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1079-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1079-123">Request headers</span></span>

| <span data-ttu-id="a1079-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a1079-124">Name</span></span>      |<span data-ttu-id="a1079-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1079-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1079-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1079-126">Authorization</span></span> | <span data-ttu-id="a1079-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1079-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1079-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1079-129">Request body</span></span>

<span data-ttu-id="a1079-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1079-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1079-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1079-131">Response</span></span>

<span data-ttu-id="a1079-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceRole](../resources/accesspackageresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1079-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1079-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1079-133">Examples</span></span>

### <a name="example-1-retrieving-the-roles-of-a-resource-for-a-group"></a><span data-ttu-id="a1079-134">Exemplo 1: Recuperando as funções de um recurso para um grupo</span><span class="sxs-lookup"><span data-stu-id="a1079-134">Example 1: Retrieving the roles of a resource for a group</span></span>

#### <a name="request"></a><span data-ttu-id="a1079-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1079-135">Request</span></span>

<span data-ttu-id="a1079-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1079-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1079-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1079-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="a1079-138">C#</span><span class="sxs-lookup"><span data-stu-id="a1079-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1079-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1079-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1079-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1079-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1079-141">Java</span><span class="sxs-lookup"><span data-stu-id="a1079-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a1079-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1079-142">Response</span></span>

<span data-ttu-id="a1079-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1079-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a1079-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1079-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-retrieve-the-roles-of-a-resource-for-a-sharepoint-online-site"></a><span data-ttu-id="a1079-145">Exemplo 2: Recuperar as funções de um recurso para um site SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a1079-145">Example 2: Retrieve the roles of a resource for a SharePoint Online site</span></span>

<span data-ttu-id="a1079-146">Este é um exemplo de recuperação das funções de um recurso, para obter a **originId** de cada função.</span><span class="sxs-lookup"><span data-stu-id="a1079-146">This is an example of retrieving the roles of a resource, to obtain the **originId** of each role.</span></span>  <span data-ttu-id="a1079-147">Isso seria usado depois que um site SharePoint Online fosse adicionado como um recurso ao catálogo, pois a **origemId** de uma função é necessária para adicionar a função a um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a1079-147">This would be used after a SharePoint Online site has been added as a resource to the catalog, as the **originId** of a role is needed to add the role to an access package.</span></span>

#### <a name="request"></a><span data-ttu-id="a1079-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1079-148">Request</span></span>

<span data-ttu-id="a1079-149">A seguir está um exemplo da solicitação, para recuperar as funções de um recurso **específico 53c71803-a0a8-4777-aecc-075de8ee3991,** que tem uma **origemSystem** do **SharePointOnline** e está localizada no catálogo **beedadfe-01d5-4025-910b-84abb936997**.</span><span class="sxs-lookup"><span data-stu-id="a1079-149">The following is an example of the request, to retrieve the roles of a particular resource **53c71803-a0a8-4777-aecc-075de8ee3991** which has an **originSystem** of **SharePointOnline** and is located in catalog **beedadfe-01d5-4025-910b-84abb9369997**.</span></span>



# <a name="http"></a>[<span data-ttu-id="a1079-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1079-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/beedadfe-01d5-4025-910b-84abb9369997/accessPackageResourceRoles?$filter=(originSystem+eq+%27SharePointOnline%27+and+accessPackageResource/id+eq+%2753c71803-a0a8-4777-aecc-075de8ee3991%27)&$select=displayName,originId
```
# <a name="c"></a>[<span data-ttu-id="a1079-151">C#</span><span class="sxs-lookup"><span data-stu-id="a1079-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1079-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1079-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1079-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1079-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1079-154">Java</span><span class="sxs-lookup"><span data-stu-id="a1079-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="a1079-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1079-155">Response</span></span>

<span data-ttu-id="a1079-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1079-156">The following is an example of the response.</span></span>  <span data-ttu-id="a1079-157">O **displayName** é o mesmo mostrado na exibição SharePoint Online de um site, e **o originId** é o identificador subjacente estabelecido pelo SharePoint Online para a função.</span><span class="sxs-lookup"><span data-stu-id="a1079-157">The **displayName** is the same as shown in the SharePoint Online view of a site, and the **originId** is the underlying identifier established by SharePoint Online for the role.</span></span>

> <span data-ttu-id="a1079-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1079-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "displayName": "Contributors",
        "originId": "4"
    },
    {
        "displayName": "Creators",
        "originId": "3"
    },
    {
        "displayName": "Viewers",
        "originId": "5"
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
