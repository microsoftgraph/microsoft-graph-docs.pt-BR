---
title: Criar accessPackageResourceRoleScope
description: Crie um novo accessPackageResourceRoleScope para adicionar uma função de recurso a um pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b4abe2f9c2c0060e97560a26c22d19ed53e01b7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466956"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="29266-103">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="29266-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="29266-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29266-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29266-105">Crie um novo [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) para adicionar uma função de recurso a um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="29266-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span> <span data-ttu-id="29266-106">O recurso do pacote de acesso, para um grupo, um aplicativo ou um site SharePoint Online, já deve existir no catálogo de pacotes de acesso e o **originId** da função de recurso recuperada da lista das funções de recurso [.](accesspackagecatalog-list-accesspackageresourceroles.md)</span><span class="sxs-lookup"><span data-stu-id="29266-106">The access package resource, for a group, an app, or a SharePoint Online site, must already exist in the access package catalog, and the **originId** for the resource role retrieved from the [list of the resource roles](accesspackagecatalog-list-accesspackageresourceroles.md).</span></span> <span data-ttu-id="29266-107">Depois de adicionar o escopo da função de recurso ao pacote de acesso, o usuário receberá essa função de recurso por meio de quaisquer atribuições de pacote de acesso atuais e futuras.</span><span class="sxs-lookup"><span data-stu-id="29266-107">Once you add the resource role scope to the access package, the user will receive this resource role through any current and future access package assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="29266-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="29266-108">Permissions</span></span>

<span data-ttu-id="29266-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29266-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29266-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29266-111">Permission type</span></span>                        | <span data-ttu-id="29266-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29266-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29266-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29266-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="29266-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29266-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="29266-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29266-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29266-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29266-116">Not supported.</span></span> |
| <span data-ttu-id="29266-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29266-117">Application</span></span>                            | <span data-ttu-id="29266-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29266-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29266-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29266-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="29266-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29266-120">Request headers</span></span>

| <span data-ttu-id="29266-121">Nome</span><span class="sxs-lookup"><span data-stu-id="29266-121">Name</span></span>          | <span data-ttu-id="29266-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="29266-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="29266-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29266-123">Authorization</span></span> | <span data-ttu-id="29266-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29266-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29266-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29266-126">Content-Type</span></span>  | <span data-ttu-id="29266-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29266-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29266-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29266-129">Request body</span></span>

<span data-ttu-id="29266-130">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="29266-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="29266-131">Inclua no objeto as relações com um objeto [accessPackageResourceRole,](../resources/accesspackageresourcerole.md) que pode ser obtido de uma solicitação para listar funções de recurso do pacote de acesso [](accesspackagecatalog-list-accesspackageresources.md) a um recurso em um [catálogo](accesspackagecatalog-list-accesspackageresourceroles.md)e um [objeto accessPackageResourceScope,](../resources/accesspackageresourcescope.md) que pode ser obtido de uma solicitação para listar recursos de pacote de acesso com `$expand=accessPackageResourceScopes` .</span><span class="sxs-lookup"><span data-stu-id="29266-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object, which can be obtained from a request to [list access package resource roles of a resource in a catalog](accesspackagecatalog-list-accesspackageresourceroles.md), and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object, which can be obtained from a request to [list access package resources](accesspackagecatalog-list-accesspackageresources.md) with `$expand=accessPackageResourceScopes`.</span></span>

## <a name="response"></a><span data-ttu-id="29266-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="29266-132">Response</span></span>

<span data-ttu-id="29266-133">Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29266-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29266-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29266-134">Examples</span></span>

### <a name="example-1-add-group-membership-as-a-resource-role-to-an-access-package"></a><span data-ttu-id="29266-135">Exemplo 1: Adicionar associação de grupo como uma função de recurso a um pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="29266-135">Example 1: Add group membership as a resource role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="29266-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29266-136">Request</span></span>

<span data-ttu-id="29266-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29266-137">The following is an example of the request.</span></span>  <span data-ttu-id="29266-138">Antes dessa solicitação, o recurso do pacote de acesso para o grupo já deve ter sido adicionado ao catálogo de pacotes de acesso `1d08498d-72a1-403f-8511-6b1f875746a0` que contém esse pacote de `b31fe1f1-3651-488f-bd9a-1711887fd4ca` acesso.</span><span class="sxs-lookup"><span data-stu-id="29266-138">Prior to this request, the access package resource `1d08498d-72a1-403f-8511-6b1f875746a0` for the group `b31fe1f1-3651-488f-bd9a-1711887fd4ca` must already have been added to the access package catalog containing this access package.</span></span>  <span data-ttu-id="29266-139">O recurso poderia ter sido adicionado ao catálogo criando uma solicitação de recurso [do pacote de acesso.](accesspackageresourcerequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="29266-139">The resource could have been added to the catalog by [creating an access package resource request](accesspackageresourcerequest-post.md).</span></span>

# <a name="http"></a>[<span data-ttu-id="29266-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="29266-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole":{
    "originId":"Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource":{"id":"1d08498d-72a1-403f-8511-6b1f875746a0","resourceType":"O365 Group","originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"}
  },
 "accessPackageResourceScope":{
   "originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"
 }
}
```
# <a name="c"></a>[<span data-ttu-id="29266-141">C#</span><span class="sxs-lookup"><span data-stu-id="29266-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29266-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29266-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29266-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29266-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29266-144">Java</span><span class="sxs-lookup"><span data-stu-id="29266-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29266-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="29266-145">Response</span></span>

<span data-ttu-id="29266-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29266-146">The following is an example of the response.</span></span>

> <span data-ttu-id="29266-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29266-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResourceRoleScopes/$entity",
    "id": "ad5c7636-e481-4528-991f-198e3b38dd56_ffd4004a-f4a9-4b22-b027-759e55c0d1db",
    "createdBy": "admin@example.com",
    "createdDateTime": "2019-12-11T01:35:26.4754081Z",
    "modifiedBy": "admin@example.com",
    "modifiedDateTime": "2019-12-11T01:35:26.4754081Z"
}
```

### <a name="example-2-add-a-sharepoint-online-site-role-to-an-access-package"></a><span data-ttu-id="29266-148">Exemplo 2: adicionar uma função de site SharePoint Online a um pacote de acesso</span><span class="sxs-lookup"><span data-stu-id="29266-148">Example 2: Add a SharePoint Online site role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="29266-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29266-149">Request</span></span>

<span data-ttu-id="29266-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29266-150">The following is an example of the request.</span></span>  <span data-ttu-id="29266-151">O recurso do pacote de acesso para o site já deve ter sido adicionado ao catálogo de pacotes de acesso que contém esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="29266-151">The access package resource for the site must already have been added to the access package catalog containing this access package.</span></span>


# <a name="http"></a>[<span data-ttu-id="29266-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="29266-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
    "accessPackageResourceRole": {
        "originId": "4",
        "originSystem": "SharePointOnline",
        "accessPackageResource": {
            "id": "53c71803-a0a8-4777-aecc-075de8ee3991"
        }
    },
    "accessPackageResourceScope": {
        "id": "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33",
        "originId": "https://microsoft.sharepoint.com/portals/Community",
        "originSystem": "SharePointOnline"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="29266-153">C#</span><span class="sxs-lookup"><span data-stu-id="29266-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29266-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29266-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29266-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29266-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29266-156">Java</span><span class="sxs-lookup"><span data-stu-id="29266-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29266-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="29266-157">Response</span></span>

<span data-ttu-id="29266-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29266-158">The following is an example of the response.</span></span>

> <span data-ttu-id="29266-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29266-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id": "6646a29e-da03-49f6-bcd9-dec124492de3_5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
