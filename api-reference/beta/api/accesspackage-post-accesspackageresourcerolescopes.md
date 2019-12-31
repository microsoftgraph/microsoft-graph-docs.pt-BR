---
title: Criar accessPackageResourceRoleScope
description: Crie um novo accessPackageResourceRoleScope para adicionar uma função de recurso a um pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a05af5bb3290a17b8e732b75f771977c5126b368
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911565"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="310d8-103">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="310d8-103">Create accessPackageResourceRoleScope</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="310d8-104">Crie um novo [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) para adicionar uma função de recurso a um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="310d8-104">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="310d8-105">O recurso de pacote de acesso já deve existir no catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="310d8-105">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="310d8-106">Todas as solicitações subsequentes de atribuição de pacote de acesso a esse pacote de acesso incluirão essa função de recurso.</span><span class="sxs-lookup"><span data-stu-id="310d8-106">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="310d8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="310d8-107">Permissions</span></span>

<span data-ttu-id="310d8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="310d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="310d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="310d8-110">Permission type</span></span>                        | <span data-ttu-id="310d8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="310d8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="310d8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="310d8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="310d8-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310d8-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="310d8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="310d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="310d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="310d8-115">Not supported.</span></span> |
| <span data-ttu-id="310d8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="310d8-116">Application</span></span>                            | <span data-ttu-id="310d8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="310d8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="310d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="310d8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="310d8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="310d8-119">Request headers</span></span>

| <span data-ttu-id="310d8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="310d8-120">Name</span></span>          | <span data-ttu-id="310d8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="310d8-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="310d8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="310d8-122">Authorization</span></span> | <span data-ttu-id="310d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="310d8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="310d8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="310d8-125">Content-Type</span></span>  | <span data-ttu-id="310d8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="310d8-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="310d8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="310d8-128">Request body</span></span>

<span data-ttu-id="310d8-129">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="310d8-129">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="310d8-130">Inclua no objeto as relações com um [accessPackageResourceRole](../resources/accesspackageresourcerole.md) e [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="310d8-130">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="310d8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="310d8-131">Response</span></span>

<span data-ttu-id="310d8-132">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="310d8-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="310d8-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="310d8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="310d8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="310d8-134">Request</span></span>

<span data-ttu-id="310d8-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="310d8-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="310d8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="310d8-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="310d8-137">C#</span><span class="sxs-lookup"><span data-stu-id="310d8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="310d8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="310d8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="310d8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="310d8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="310d8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="310d8-140">Response</span></span>

<span data-ttu-id="310d8-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="310d8-141">The following is an example of the response.</span></span>

> <span data-ttu-id="310d8-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="310d8-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
