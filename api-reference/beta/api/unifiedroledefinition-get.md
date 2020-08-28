---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 96959392b98408cad9e20a280b3800290df63f63
ms.sourcegitcommit: 4a37678913c98f62b8174de6ca03908b9af864bd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/28/2020
ms.locfileid: "47296537"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="ee359-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ee359-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="ee359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee359-105">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ee359-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="ee359-106">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="ee359-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee359-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee359-107">Permissions</span></span>

<span data-ttu-id="ee359-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee359-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee359-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee359-110">Permission type</span></span>      | <span data-ttu-id="ee359-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee359-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee359-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee359-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee359-113">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ee359-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee359-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee359-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee359-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee359-115">Not supported.</span></span>    |
|<span data-ttu-id="ee359-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee359-116">Application</span></span> | <span data-ttu-id="ee359-117">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ee359-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee359-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee359-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee359-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee359-119">Optional query parameters</span></span>

<span data-ttu-id="ee359-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee359-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee359-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee359-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee359-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee359-122">Request headers</span></span>

| <span data-ttu-id="ee359-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ee359-123">Name</span></span>      |<span data-ttu-id="ee359-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee359-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee359-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee359-125">Authorization</span></span> | <span data-ttu-id="ee359-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ee359-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee359-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee359-127">Request body</span></span>

<span data-ttu-id="ee359-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee359-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee359-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee359-129">Response</span></span>

<span data-ttu-id="ee359-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee359-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee359-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee359-131">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role"></a><span data-ttu-id="ee359-132">Exemplo 1: obter a definição de uma função personalizada</span><span class="sxs-lookup"><span data-stu-id="ee359-132">Example 1: Get the definition of a custom role</span></span>

#### <a name="request"></a><span data-ttu-id="ee359-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee359-133">Request</span></span>

<span data-ttu-id="ee359-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee359-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee359-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee359-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="ee359-136">C#</span><span class="sxs-lookup"><span data-stu-id="ee359-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee359-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee359-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee359-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee359-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee359-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee359-139">Response</span></span>

<span data-ttu-id="ee359-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee359-140">The following is an example of the response.</span></span>

> <span data-ttu-id="ee359-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee359-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "f189965f-f560-4c59-9101-933d4c87a91a",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f189965f-f560-4c59-9101-933d4c87a91a')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

### <a name="example-2-get-the-definition-of-a-built-in-role"></a><span data-ttu-id="ee359-143">Exemplo 2: obter a definição de uma função interna</span><span class="sxs-lookup"><span data-stu-id="ee359-143">Example 2: Get the definition of a built-in role</span></span>

#### <a name="request"></a><span data-ttu-id="ee359-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee359-144">Request</span></span>

<span data-ttu-id="ee359-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee359-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```

---


#### <a name="response"></a><span data-ttu-id="ee359-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee359-146">Response</span></span>

<span data-ttu-id="ee359-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee359-147">The following is an example of the response.</span></span>

> <span data-ttu-id="ee359-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee359-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
        }
    ]
}
```
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="ee359-150">Exemplo 3: obter a definição de uma função interna do Azure AD e $expand na função herdada de</span><span class="sxs-lookup"><span data-stu-id="ee359-150">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="ee359-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee359-151">Request</span></span>

<span data-ttu-id="ee359-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee359-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```

---


#### <a name="response"></a><span data-ttu-id="ee359-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee359-153">Response</span></span>

<span data-ttu-id="ee359-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee359-154">The following is an example of the response.</span></span>

> <span data-ttu-id="ee359-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee359-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions(inheritsPermissionsFrom())/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
            "displayName": "Directory Readers",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/administrativeUnits/standard/read",
                        "microsoft.directory/administrativeUnits/members/read",
                        "microsoft.directory/applications/standard/read",
                        "microsoft.directory/applications/owners/read",
                        "microsoft.directory/applications/policies/read",
                        "microsoft.directory/contacts/standard/read",
                        "microsoft.directory/contacts/memberOf/read",
                        "microsoft.directory/contracts/standard/read",
                        "microsoft.directory/devices/standard/read",
                        "microsoft.directory/devices/memberOf/read",
                        "microsoft.directory/devices/registeredOwners/read",
                        "microsoft.directory/devices/registeredUsers/read",
                        "microsoft.directory/directoryRoles/standard/read",
                        "microsoft.directory/directoryRoles/eligibleMembers/read",
                        "microsoft.directory/directoryRoles/members/read",
                        "microsoft.directory/domains/standard/read",
                        "microsoft.directory/groups/standard/read",
                        "microsoft.directory/groups/appRoleAssignments/read",
                        "microsoft.directory/groups/memberOf/read",
                        "microsoft.directory/groups/members/read",
                        "microsoft.directory/groups/owners/read",
                        "microsoft.directory/groups/settings/read",
                        "microsoft.directory/groupSettings/standard/read",
                        "microsoft.directory/groupSettingTemplates/standard/read",
                        "microsoft.directory/oAuth2PermissionGrants/standard/read",
                        "microsoft.directory/organization/standard/read",
                        "microsoft.directory/organization/trustedCAsForPasswordlessAuth/read",
                        "microsoft.directory/applicationPolicies/standard/read",
                        "microsoft.directory/roleAssignments/standard/read",
                        "microsoft.directory/roleDefinitions/standard/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignedTo/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignments/read",
                        "microsoft.directory/servicePrincipals/standard/read",
                        "microsoft.directory/servicePrincipals/memberOf/read",
                        "microsoft.directory/servicePrincipals/oAuth2PermissionGrants/read",
                        "microsoft.directory/servicePrincipals/owners/read",
                        "microsoft.directory/servicePrincipals/ownedObjects/read",
                        "microsoft.directory/servicePrincipals/policies/read",
                        "microsoft.directory/subscribedSkus/standard/read",
                        "microsoft.directory/users/standard/read",
                        "microsoft.directory/users/appRoleAssignments/read",
                        "microsoft.directory/users/directReports/read",
                        "microsoft.directory/users/manager/read",
                        "microsoft.directory/users/memberOf/read",
                        "microsoft.directory/users/oAuth2PermissionGrants/read",
                        "microsoft.directory/users/ownedDevices/read",
                        "microsoft.directory/users/ownedObjects/read",
                        "microsoft.directory/users/registeredDevices/read"
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
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
