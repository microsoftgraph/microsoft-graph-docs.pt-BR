---
title: Criar accessPackageResourceRoleScope
description: Crie um novo accessPackageResourceRoleScope para adicionar uma função de recurso a um pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ffaedc45cc512b554fda3ce4dd06794fba716b16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439804"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="37c31-103">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="37c31-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="37c31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c31-105">Crie um novo [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) para adicionar uma função de recurso a um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="37c31-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="37c31-106">O recurso do pacote de acesso já deve existir no catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="37c31-106">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="37c31-107">Qualquer solicitação de atribuição de pacote de acesso subsequente a esse pacote de acesso incluirá essa função de recurso.</span><span class="sxs-lookup"><span data-stu-id="37c31-107">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="37c31-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="37c31-108">Permissions</span></span>

<span data-ttu-id="37c31-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37c31-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37c31-111">Permission type</span></span>                        | <span data-ttu-id="37c31-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37c31-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37c31-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37c31-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="37c31-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c31-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="37c31-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37c31-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37c31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37c31-116">Not supported.</span></span> |
| <span data-ttu-id="37c31-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37c31-117">Application</span></span>                            | <span data-ttu-id="37c31-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c31-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37c31-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37c31-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="37c31-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37c31-120">Request headers</span></span>

| <span data-ttu-id="37c31-121">Nome</span><span class="sxs-lookup"><span data-stu-id="37c31-121">Name</span></span>          | <span data-ttu-id="37c31-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c31-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37c31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37c31-123">Authorization</span></span> | <span data-ttu-id="37c31-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c31-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37c31-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37c31-126">Content-Type</span></span>  | <span data-ttu-id="37c31-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37c31-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37c31-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37c31-129">Request body</span></span>

<span data-ttu-id="37c31-130">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="37c31-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="37c31-131">Inclua no objeto as relações com [um accessPackageResourceRole](../resources/accesspackageresourcerole.md) e [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="37c31-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="37c31-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c31-132">Response</span></span>

<span data-ttu-id="37c31-133">Se tiver êxito, este método retornará um código de resposta de 200 séries e um novo [objeto accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37c31-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37c31-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37c31-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37c31-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37c31-135">Request</span></span>

<span data-ttu-id="37c31-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37c31-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37c31-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c31-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="37c31-138">C#</span><span class="sxs-lookup"><span data-stu-id="37c31-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c31-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c31-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c31-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c31-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c31-141">Java</span><span class="sxs-lookup"><span data-stu-id="37c31-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37c31-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="37c31-142">Response</span></span>

<span data-ttu-id="37c31-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37c31-143">The following is an example of the response.</span></span>

> <span data-ttu-id="37c31-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37c31-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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


