---
title: Criar accessPackageResourceRoleScope
description: Crie um novo accessPackageResourceRoleScope para adicionar uma função de recurso a um pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9dd99fcbeea0f735938c0a4661da89afa9c83d6f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871714"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="0de26-103">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="0de26-103">Create accessPackageResourceRoleScope</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0de26-104">Crie um novo [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) para adicionar uma função de recurso a um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="0de26-104">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span>  <span data-ttu-id="0de26-105">O recurso de pacote de acesso já deve existir no catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="0de26-105">The access package resource must already exist in the access package catalog.</span></span>  <span data-ttu-id="0de26-106">Todas as solicitações subsequentes de atribuição de pacote de acesso a esse pacote de acesso incluirão essa função de recurso.</span><span class="sxs-lookup"><span data-stu-id="0de26-106">Any subsequent access package assignment requests to this access package will include this resource role.</span></span>  

## <a name="permissions"></a><span data-ttu-id="0de26-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0de26-107">Permissions</span></span>

<span data-ttu-id="0de26-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0de26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0de26-110">Permission type</span></span>                        | <span data-ttu-id="0de26-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0de26-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0de26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0de26-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0de26-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de26-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0de26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0de26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0de26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de26-115">Not supported.</span></span> |
| <span data-ttu-id="0de26-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0de26-116">Application</span></span>                            | <span data-ttu-id="0de26-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de26-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0de26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0de26-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="0de26-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0de26-119">Request headers</span></span>

| <span data-ttu-id="0de26-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0de26-120">Name</span></span>          | <span data-ttu-id="0de26-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0de26-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0de26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0de26-122">Authorization</span></span> | <span data-ttu-id="0de26-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de26-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0de26-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0de26-125">Content-Type</span></span>  | <span data-ttu-id="0de26-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de26-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0de26-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0de26-128">Request body</span></span>

<span data-ttu-id="0de26-129">No corpo da solicitação, forneça uma representação JSON de um objeto [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="0de26-129">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="0de26-130">Inclua no objeto as relações com um [accessPackageResourceRole](../resources/accesspackageresourcerole.md) e [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="0de26-130">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>  

## <a name="response"></a><span data-ttu-id="0de26-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de26-131">Response</span></span>

<span data-ttu-id="0de26-132">Se tiver êxito, este método retornará um código de resposta de série 200 e um novo objeto [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0de26-132">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0de26-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0de26-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0de26-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de26-134">Request</span></span>

<span data-ttu-id="0de26-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de26-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0de26-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de26-136">Response</span></span>

<span data-ttu-id="0de26-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de26-137">The following is an example of the response.</span></span>

> <span data-ttu-id="0de26-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0de26-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
