---
title: Listar unifiedRoleDefinitions
description: Obter uma lista de objetos unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 58d8ca676a3462818e82e69d4ab344ec0479514d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442245"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="b6bed-103">Listar unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="b6bed-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="b6bed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6bed-105">Obter uma lista de [objetos unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="b6bed-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="b6bed-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="b6bed-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="b6bed-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="b6bed-107">cloud PC</span></span> 
- <span data-ttu-id="b6bed-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="b6bed-108">device management (Intune)</span></span>
- <span data-ttu-id="b6bed-109">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="b6bed-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="b6bed-110">gerenciamento de direitos (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="b6bed-110">entitlement management (Azure AD)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="b6bed-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="b6bed-111">Permissions</span></span>

<span data-ttu-id="b6bed-112">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b6bed-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="b6bed-113">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bed-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="b6bed-114">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="b6bed-114">For Cloud PC provider</span></span>

|<span data-ttu-id="b6bed-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bed-115">Permission type</span></span>      | <span data-ttu-id="b6bed-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bed-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6bed-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bed-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="b6bed-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="b6bed-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bed-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6bed-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bed-120">Not supported.</span></span>    |
|<span data-ttu-id="b6bed-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bed-121">Application</span></span> | <span data-ttu-id="b6bed-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="b6bed-123">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="b6bed-123">For Device management (Intune) provider</span></span>

|<span data-ttu-id="b6bed-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bed-124">Permission type</span></span>      | <span data-ttu-id="b6bed-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bed-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6bed-126">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bed-126">Delegated (work or school account)</span></span> |  <span data-ttu-id="b6bed-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="b6bed-128">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bed-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6bed-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bed-129">Not supported.</span></span>    |
|<span data-ttu-id="b6bed-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bed-130">Application</span></span> | <span data-ttu-id="b6bed-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="b6bed-132">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="b6bed-132">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="b6bed-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bed-133">Permission type</span></span>      | <span data-ttu-id="b6bed-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bed-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6bed-135">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bed-135">Delegated (work or school account)</span></span> |  <span data-ttu-id="b6bed-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="b6bed-137">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bed-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6bed-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bed-138">Not supported.</span></span>    |
|<span data-ttu-id="b6bed-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bed-139">Application</span></span> | <span data-ttu-id="b6bed-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="b6bed-141">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="b6bed-141">For Entitlement management provider</span></span>

|<span data-ttu-id="b6bed-142">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bed-142">Permission type</span></span>      | <span data-ttu-id="b6bed-143">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bed-143">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6bed-144">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bed-144">Delegated (work or school account)</span></span> |  <span data-ttu-id="b6bed-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bed-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="b6bed-146">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bed-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6bed-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bed-147">Not supported.</span></span>    |
|<span data-ttu-id="b6bed-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bed-148">Application</span></span> | <span data-ttu-id="b6bed-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bed-149">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6bed-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bed-150">HTTP request</span></span>

<span data-ttu-id="b6bed-151">Para listar definições de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="b6bed-151">To list role definitions for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions
```

<span data-ttu-id="b6bed-152">Para listar definições de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="b6bed-152">To list role definitions for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="b6bed-153">Para listar definições de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="b6bed-153">To list role definitions for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/directory/roleDefinitions
```

<span data-ttu-id="b6bed-154">Para listar definições de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="b6bed-154">To list role definitions for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/entitlementManagement/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6bed-155">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6bed-155">Optional query parameters</span></span>
<span data-ttu-id="b6bed-156">Este método dá `$filter` suporte ao parâmetro de consulta em , e `id` `displayName` `isBuiltIn` propriedades.</span><span class="sxs-lookup"><span data-stu-id="b6bed-156">This method supports `$filter` query parameter on `id`, `displayName`, and `isBuiltIn` properties.</span></span> <span data-ttu-id="b6bed-157">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6bed-157">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6bed-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bed-158">Request headers</span></span>

| <span data-ttu-id="b6bed-159">Nome</span><span class="sxs-lookup"><span data-stu-id="b6bed-159">Name</span></span>      |<span data-ttu-id="b6bed-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6bed-160">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6bed-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6bed-161">Authorization</span></span> | <span data-ttu-id="b6bed-162">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b6bed-162">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6bed-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bed-163">Request body</span></span>

<span data-ttu-id="b6bed-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6bed-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6bed-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bed-165">Response</span></span>

<span data-ttu-id="b6bed-166">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bed-166">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6bed-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b6bed-167">Examples</span></span>

### <a name="example-1-list-role-definitions-for-a-directory-provider"></a><span data-ttu-id="b6bed-168">Exemplo 1: Listar definições de função para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="b6bed-168">Example 1: List role definitions for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="b6bed-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bed-169">Request</span></span>

<span data-ttu-id="b6bed-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bed-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6bed-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bed-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_directory"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="b6bed-172">C#</span><span class="sxs-lookup"><span data-stu-id="b6bed-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6bed-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6bed-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6bed-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6bed-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6bed-175">Java</span><span class="sxs-lookup"><span data-stu-id="b6bed-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6bed-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bed-176">Response</span></span>

<span data-ttu-id="b6bed-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bed-177">The following is an example of the response.</span></span>

> <span data-ttu-id="b6bed-178">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6bed-178">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_directory",
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
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
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
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
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
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

### <a name="example-2-list-role-definitions-for-a-cloud-pc-provider"></a><span data-ttu-id="b6bed-179">Exemplo 2: Listar definições de função para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="b6bed-179">Example 2: List role definitions for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="b6bed-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bed-180">Request</span></span>

<span data-ttu-id="b6bed-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bed-181">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6bed-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bed-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_cloudpc"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="b6bed-183">C#</span><span class="sxs-lookup"><span data-stu-id="b6bed-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6bed-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6bed-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6bed-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6bed-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6bed-186">Java</span><span class="sxs-lookup"><span data-stu-id="b6bed-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6bed-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bed-187">Response</span></span>

<span data-ttu-id="b6bed-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bed-188">The following is an example of the response.</span></span>

> <span data-ttu-id="b6bed-189">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6bed-189">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_cloudpc",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions",
    "value": [
        {
            "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "description": "Cloud PC Administrator has read and write access to all Cloud PC features located within the Cloud PC blade.",
            "displayName": "Cloud PC Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "version": null,
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "Microsoft.CloudPC/CloudPCs/Read",
                        "Microsoft.CloudPC/CloudPCs/Reprovision",
                        "Microsoft.CloudPC/DeviceImages/Create",
                        "Microsoft.CloudPC/DeviceImages/Delete",
                        "Microsoft.CloudPC/DeviceImages/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Create",
                        "Microsoft.CloudPC/OnPremisesConnections/Delete",
                        "Microsoft.CloudPC/OnPremisesConnections/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Update",
                        "Microsoft.CloudPC/OnPremisesConnections/RunHealthChecks",
                        "Microsoft.CloudPC/OnPremisesConnections/UpdateAdDomainPassword",
                        "Microsoft.CloudPC/ProvisioningPolicies/Assign",
                        "Microsoft.CloudPC/ProvisioningPolicies/Create",
                        "Microsoft.CloudPC/ProvisioningPolicies/Delete",
                        "Microsoft.CloudPC/ProvisioningPolicies/Read",
                        "Microsoft.CloudPC/ProvisioningPolicies/Update",
                        "Microsoft.CloudPC/RoleAssignments/Create",
                        "Microsoft.CloudPC/RoleAssignments/Update",
                        "Microsoft.CloudPC/RoleAssignments/Delete",
                        "Microsoft.CloudPC/Roles/Read"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
            "description": "Cloud PC Reader has read access to all Cloud PC features located within the Cloud PC blade.",
            "displayName": "Cloud PC Reader",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
            "version": null,
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "Microsoft.CloudPC/CloudPCs/Read",
                        "Microsoft.CloudPC/DeviceImages/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Read",
                        "Microsoft.CloudPC/ProvisioningPolicies/Read",
                        "Microsoft.CloudPC/Roles/Read"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

### <a name="example-3-list-role-definitions-for-the-entitlement-management-provider"></a><span data-ttu-id="b6bed-190">Exemplo 3: Listar definições de função para o provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="b6bed-190">Example 3: List role definitions for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="b6bed-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bed-191">Request</span></span>

<span data-ttu-id="b6bed-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bed-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b6bed-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bed-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_entitlementmanagement"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="b6bed-194">C#</span><span class="sxs-lookup"><span data-stu-id="b6bed-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-entitlementmanagement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6bed-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6bed-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-entitlementmanagement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6bed-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6bed-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-entitlementmanagement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6bed-197">Java</span><span class="sxs-lookup"><span data-stu-id="b6bed-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-entitlementmanagement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b6bed-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bed-198">Response</span></span>

<span data-ttu-id="b6bed-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bed-199">The following is an example of the response.</span></span>

> <span data-ttu-id="b6bed-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6bed-200">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_entitlementmanagement",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleDefinitions",
    "value": [
        {
            "id": "ae79f266-94d4-4dab-b730-feca7e132178",
            "displayName": "Catalog owner",
            "description": "Catalog owner",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "ae79f266-94d4-4dab-b730-feca7e132178",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/allTasks"
                    ]
                }
            ]
        },
        {
            "id": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "displayName": "Catalog reader",
            "description": "Catalog reader",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/Read"
                    ]
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


