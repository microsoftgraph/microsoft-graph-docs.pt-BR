---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e as relações de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9626695a5ad9fce18b14c25fcca75fe394d5a816
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440691"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="36083-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="36083-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="36083-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36083-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36083-105">Obter as propriedades e as relações de [um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="36083-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="36083-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="36083-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="36083-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="36083-107">cloud PC</span></span> 
- <span data-ttu-id="36083-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="36083-108">device management (Intune)</span></span>
- <span data-ttu-id="36083-109">directory (funções de diretório do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="36083-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="36083-110">gerenciamento de direitos (gerenciamento de direitos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="36083-110">entitlement management (Azure AD entitlement management)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="36083-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="36083-111">Permissions</span></span>

<span data-ttu-id="36083-112">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="36083-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="36083-113">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36083-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="36083-114">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="36083-114">For Cloud PC provider</span></span>

|<span data-ttu-id="36083-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36083-115">Permission type</span></span>      | <span data-ttu-id="36083-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36083-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36083-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36083-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="36083-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="36083-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36083-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36083-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36083-120">Not supported.</span></span>    |
|<span data-ttu-id="36083-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36083-121">Application</span></span> | <span data-ttu-id="36083-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="36083-123">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="36083-123">For Device management (Intune) provider</span></span>

|<span data-ttu-id="36083-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36083-124">Permission type</span></span>      | <span data-ttu-id="36083-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36083-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36083-126">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36083-126">Delegated (work or school account)</span></span> |  <span data-ttu-id="36083-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="36083-128">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36083-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36083-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36083-129">Not supported.</span></span>    |
|<span data-ttu-id="36083-130">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36083-130">Application</span></span> | <span data-ttu-id="36083-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="36083-132">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="36083-132">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="36083-133">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36083-133">Permission type</span></span>      | <span data-ttu-id="36083-134">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36083-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36083-135">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36083-135">Delegated (work or school account)</span></span> |  <span data-ttu-id="36083-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36083-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="36083-137">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36083-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36083-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36083-138">Not supported.</span></span>    |
|<span data-ttu-id="36083-139">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36083-139">Application</span></span> | <span data-ttu-id="36083-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="36083-141">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="36083-141">For Entitlement management provider</span></span>

|<span data-ttu-id="36083-142">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36083-142">Permission type</span></span>      | <span data-ttu-id="36083-143">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36083-143">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36083-144">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36083-144">Delegated (work or school account)</span></span> |  <span data-ttu-id="36083-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36083-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="36083-146">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36083-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36083-147">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36083-147">Not supported.</span></span>    |
|<span data-ttu-id="36083-148">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36083-148">Application</span></span> | <span data-ttu-id="36083-149">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36083-149">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36083-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-150">HTTP request</span></span>

<span data-ttu-id="36083-151">Obter uma definição de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="36083-151">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="36083-152">Obter uma definição de função para um provedor de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="36083-152">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="36083-153">Obter uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="36083-153">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

<span data-ttu-id="36083-154">Obter uma definição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="36083-154">Get a role definition for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36083-155">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36083-155">Optional query parameters</span></span>

<span data-ttu-id="36083-156">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36083-156">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="36083-157">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="36083-157">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36083-158">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-158">Request headers</span></span>

| <span data-ttu-id="36083-159">Nome</span><span class="sxs-lookup"><span data-stu-id="36083-159">Name</span></span>      |<span data-ttu-id="36083-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="36083-160">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36083-161">Autorização</span><span class="sxs-lookup"><span data-stu-id="36083-161">Authorization</span></span> | <span data-ttu-id="36083-162">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="36083-162">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="36083-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-163">Request body</span></span>

<span data-ttu-id="36083-164">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36083-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36083-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-165">Response</span></span>

<span data-ttu-id="36083-166">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36083-166">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36083-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36083-167">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="36083-168">Exemplo 1: Obter a definição de uma função personalizada para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="36083-168">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="36083-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-169">Request</span></span>

<span data-ttu-id="36083-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36083-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36083-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="36083-172">C#</span><span class="sxs-lookup"><span data-stu-id="36083-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36083-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36083-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36083-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36083-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36083-175">Java</span><span class="sxs-lookup"><span data-stu-id="36083-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="36083-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-176">Response</span></span>

<span data-ttu-id="36083-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36083-177">The following is an example of the response.</span></span>

> <span data-ttu-id="36083-178">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36083-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="36083-179">Exemplo 2: Obter a definição de uma função embutida para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="36083-179">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="36083-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-180">Request</span></span>

<span data-ttu-id="36083-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36083-181">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36083-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="36083-183">C#</span><span class="sxs-lookup"><span data-stu-id="36083-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36083-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36083-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36083-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36083-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36083-186">Java</span><span class="sxs-lookup"><span data-stu-id="36083-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="36083-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-187">Response</span></span>

<span data-ttu-id="36083-188">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36083-188">The following is an example of the response.</span></span>

> <span data-ttu-id="36083-189">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36083-189">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="36083-190">Exemplo 3: Obter a definição de uma função do Azure AD e $expand na função herdada de</span><span class="sxs-lookup"><span data-stu-id="36083-190">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="36083-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-191">Request</span></span>

<span data-ttu-id="36083-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36083-192">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36083-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="36083-194">C#</span><span class="sxs-lookup"><span data-stu-id="36083-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36083-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36083-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36083-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36083-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36083-197">Java</span><span class="sxs-lookup"><span data-stu-id="36083-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="36083-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-198">Response</span></span>

<span data-ttu-id="36083-199">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36083-199">The following is an example of the response.</span></span>

> <span data-ttu-id="36083-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="36083-200">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="36083-201">Exemplo 4: Obter a definição de uma função criada para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="36083-201">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="36083-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-202">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36083-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="36083-204">C#</span><span class="sxs-lookup"><span data-stu-id="36083-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36083-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36083-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36083-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36083-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36083-207">Java</span><span class="sxs-lookup"><span data-stu-id="36083-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="36083-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-208">Response</span></span>
> <span data-ttu-id="36083-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36083-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions/$entity",
    "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
    "description": "Have read-only access all Cloud PC features.",
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
                "Microsoft.CloudPC/Roles/Read",
                "Microsoft.CloudPC/SelfServiceSettings/Read"
            ],
            "condition": null
        }
    ]
}
```

## <a name="example-5-get-the-definition-of-a-built-in-role-for-the-entitlement-management-provider"></a><span data-ttu-id="36083-211">Exemplo 5: Obter a definição de uma função integrado para o provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="36083-211">Example 5: Get the definition of a built-in role for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="36083-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36083-212">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36083-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="36083-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_entitlementmanagement_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8
```
# <a name="c"></a>[<span data-ttu-id="36083-214">C#</span><span class="sxs-lookup"><span data-stu-id="36083-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-entitlementmanagement-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36083-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36083-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-entitlementmanagement-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36083-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36083-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-entitlementmanagement-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36083-217">Java</span><span class="sxs-lookup"><span data-stu-id="36083-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-entitlementmanagement-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="36083-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="36083-218">Response</span></span>
> <span data-ttu-id="36083-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36083-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleDefinitions/$entity",
    "id": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "displayName": "Catalog creator",
    "description": "Catalog creator",
    "isBuiltIn": true,
    "isEnabled": true,
    "templateId": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "version": "1.0",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.entitlementManagement/AccessPackageCatalog/Create"
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


