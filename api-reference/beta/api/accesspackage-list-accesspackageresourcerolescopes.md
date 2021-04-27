---
title: Listar accessPackageResourceRoleScopes
description: Recupere uma lista de objetos accesspackageresourcerolescope.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d2376d9eb4aaf0bd8ab58b0dd5cbbb131e36a01c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038632"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="48db1-103">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="48db1-103">List accessPackageResourceRoleScopes</span></span>

<span data-ttu-id="48db1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48db1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48db1-105">Recupere um pacote de acesso com uma lista [de objetos accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="48db1-105">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="48db1-106">Cada objeto é links para [um accessPackageResourceRole](../resources/accesspackageresourcerole.md) e [um accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="48db1-106">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48db1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="48db1-107">Permissions</span></span>

<span data-ttu-id="48db1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48db1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48db1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48db1-110">Permission type</span></span>                        | <span data-ttu-id="48db1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48db1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48db1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48db1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="48db1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48db1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="48db1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48db1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48db1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48db1-115">Not supported.</span></span> |
| <span data-ttu-id="48db1-116">Application</span><span class="sxs-lookup"><span data-stu-id="48db1-116">Application</span></span>                            | <span data-ttu-id="48db1-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48db1-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48db1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48db1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48db1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="48db1-119">Optional query parameters</span></span>

<span data-ttu-id="48db1-120">Este método usa parâmetros de consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48db1-120">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="48db1-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="48db1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="48db1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48db1-122">Request headers</span></span>

| <span data-ttu-id="48db1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="48db1-123">Name</span></span>      |<span data-ttu-id="48db1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="48db1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48db1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="48db1-125">Authorization</span></span> | <span data-ttu-id="48db1-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48db1-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48db1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48db1-128">Request body</span></span>

<span data-ttu-id="48db1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48db1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48db1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="48db1-130">Response</span></span>

<span data-ttu-id="48db1-131">Se tiver êxito, este método retornará um código de resposta e um accessPackage contendo uma coleção de objetos `200 OK` [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) no corpo da resposta. [](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="48db1-131">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48db1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48db1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48db1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48db1-133">Request</span></span>

<span data-ttu-id="48db1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48db1-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48db1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="48db1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="c"></a>[<span data-ttu-id="48db1-136">C#</span><span class="sxs-lookup"><span data-stu-id="48db1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48db1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48db1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48db1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48db1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48db1-139">Java</span><span class="sxs-lookup"><span data-stu-id="48db1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerolescopes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48db1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="48db1-140">Response</span></span>

<span data-ttu-id="48db1-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48db1-141">The following is an example of the response.</span></span>

> <span data-ttu-id="48db1-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="48db1-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "id": "933a4822-aed1-445b-9623-62116cd07a39",
    "catalogId": "32efb28c-9a7a-446c-986b-ca6528c6669d",
    "displayName": "Test Package 9-9",
    "description": "Test Package 9-9",
    "isHidden": false,
    "accessPackageResourceRoleScopes": [
        {
            "id": "70113acf-4dcb-453f-b517-2394598d974e_22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
            "createdBy": "alice@contoso.com",
            "createdDateTime": "2019-09-09T19:54:14.853Z",
            "modifiedBy": "alice@contoso.com",
            "modifiedDateTime": "2019-09-09T19:54:14.853Z",
            "accessPackageResourceRole": {
                "id": "70113acf-4dcb-453f-b517-2394598d974e",
                "displayName": "Owner",
                "originSystem": "origin-type",
                "originId": "Owner_7b56ede0-9b58-40bd-b11e-b3d18fc32698"
            },
            "accessPackageResourceScope": {
                "id": "22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
                "displayName": "Root",
                "description": "Root Scope",
                "originId": "7b56ede0-9b58-40bd-b11e-b3d18fc32698",
                "originSystem": "origin-type",
                "isRootScope": true
            }
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoleScopes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


