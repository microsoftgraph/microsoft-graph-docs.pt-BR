---
title: Listar unifiedRoleDefinitions
description: Obtenha uma lista de objetos unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 779a8dfcc582b37118b975914141d0508860f9a5
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43216761"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="26d4b-103">Listar unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="26d4b-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="26d4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d4b-105">Obtenha uma lista de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="26d4b-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="26d4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26d4b-106">Permissions</span></span>

<span data-ttu-id="26d4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26d4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26d4b-109">Permission type</span></span>      | <span data-ttu-id="26d4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26d4b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26d4b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26d4b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26d4b-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="26d4b-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26d4b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26d4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26d4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26d4b-114">Not supported.</span></span>    |
|<span data-ttu-id="26d4b-115">Application</span><span class="sxs-lookup"><span data-stu-id="26d4b-115">Application</span></span> | <span data-ttu-id="26d4b-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="26d4b-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26d4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26d4b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26d4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="26d4b-118">Optional query parameters</span></span>
<span data-ttu-id="26d4b-119">Este método é `$filter` compatível `id`com `displayName`o, `isBuiltIn`, e.</span><span class="sxs-lookup"><span data-stu-id="26d4b-119">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="26d4b-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="26d4b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="26d4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26d4b-121">Request headers</span></span>

| <span data-ttu-id="26d4b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="26d4b-122">Name</span></span>      |<span data-ttu-id="26d4b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="26d4b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="26d4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="26d4b-124">Authorization</span></span> | <span data-ttu-id="26d4b-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="26d4b-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26d4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26d4b-126">Request body</span></span>

<span data-ttu-id="26d4b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26d4b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26d4b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d4b-128">Response</span></span>

<span data-ttu-id="26d4b-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26d4b-129">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26d4b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26d4b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="26d4b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26d4b-131">Request</span></span>

<span data-ttu-id="26d4b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26d4b-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="26d4b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d4b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="26d4b-134">C#</span><span class="sxs-lookup"><span data-stu-id="26d4b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26d4b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26d4b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26d4b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26d4b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26d4b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="26d4b-137">Response</span></span>

<span data-ttu-id="26d4b-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="26d4b-138">The following is an example of the response.</span></span>

> <span data-ttu-id="26d4b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26d4b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
