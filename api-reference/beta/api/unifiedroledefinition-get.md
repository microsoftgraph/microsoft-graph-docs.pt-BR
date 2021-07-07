---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e as relações de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 07b9aff276c46fbdcca56b365d11e7ac12066408
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317074"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="e5223-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e5223-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="e5223-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5223-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5223-105">Obter as propriedades e as relações de [um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="e5223-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="e5223-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="e5223-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e5223-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="e5223-107">cloud PC</span></span> 
- <span data-ttu-id="e5223-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="e5223-108">device management (Intune)</span></span>
- <span data-ttu-id="e5223-109">directory (funções de diretório do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="e5223-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="e5223-110">gerenciamento de direitos (gerenciamento de direitos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="e5223-110">entitlement management (Azure AD entitlement management)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e5223-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5223-111">Permissions</span></span>

<span data-ttu-id="e5223-112">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e5223-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e5223-113">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5223-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="e5223-114">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="e5223-114">Supported provider</span></span>      | <span data-ttu-id="e5223-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5223-115">Delegated (work or school account)</span></span>  | <span data-ttu-id="e5223-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5223-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5223-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5223-117">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="e5223-118">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="e5223-118">Cloud PC</span></span> | <span data-ttu-id="e5223-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="e5223-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5223-120">Not supported.</span></span> | <span data-ttu-id="e5223-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="e5223-122">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5223-122">Device management</span></span> | <span data-ttu-id="e5223-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="e5223-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5223-124">Not supported.</span></span> | <span data-ttu-id="e5223-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e5223-126">Diretório</span><span class="sxs-lookup"><span data-stu-id="e5223-126">Directory</span></span> | <span data-ttu-id="e5223-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5223-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e5223-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5223-128">Not supported.</span></span>| <span data-ttu-id="e5223-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="e5223-130">Gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="e5223-130">Entitlement management</span></span> | <span data-ttu-id="e5223-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5223-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="e5223-132">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5223-132">Not supported.</span></span> | <span data-ttu-id="e5223-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5223-133">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5223-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5223-134">HTTP request</span></span>

<span data-ttu-id="e5223-135">Obter uma definição de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="e5223-135">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="e5223-136">Obter uma definição de função para um provedor de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="e5223-136">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="e5223-137">Obter uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="e5223-137">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

<span data-ttu-id="e5223-138">Obter uma definição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="e5223-138">Get a role definition for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5223-139">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5223-139">Optional query parameters</span></span>

<span data-ttu-id="e5223-140">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5223-140">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="e5223-141">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e5223-141">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5223-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-142">Request headers</span></span>

| <span data-ttu-id="e5223-143">Nome</span><span class="sxs-lookup"><span data-stu-id="e5223-143">Name</span></span>      |<span data-ttu-id="e5223-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5223-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5223-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5223-145">Authorization</span></span> | <span data-ttu-id="e5223-146">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e5223-146">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5223-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-147">Request body</span></span>

<span data-ttu-id="e5223-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5223-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5223-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-149">Response</span></span>

<span data-ttu-id="e5223-150">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5223-150">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5223-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5223-151">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="e5223-152">Exemplo 1: Obter a definição de uma função personalizada para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="e5223-152">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5223-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-153">Request</span></span>

<span data-ttu-id="e5223-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5223-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5223-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5223-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="e5223-156">C#</span><span class="sxs-lookup"><span data-stu-id="e5223-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5223-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5223-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5223-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5223-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5223-159">Java</span><span class="sxs-lookup"><span data-stu-id="e5223-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5223-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-160">Response</span></span>

<span data-ttu-id="e5223-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5223-161">The following is an example of the response.</span></span>

> <span data-ttu-id="e5223-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5223-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="e5223-163">Exemplo 2: Obter a definição de uma função embutida para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="e5223-163">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5223-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-164">Request</span></span>

<span data-ttu-id="e5223-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5223-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5223-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5223-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="e5223-167">C#</span><span class="sxs-lookup"><span data-stu-id="e5223-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5223-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5223-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5223-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5223-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5223-170">Java</span><span class="sxs-lookup"><span data-stu-id="e5223-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="e5223-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-171">Response</span></span>

<span data-ttu-id="e5223-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5223-172">The following is an example of the response.</span></span>

> <span data-ttu-id="e5223-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5223-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="e5223-174">Exemplo 3: Obter a definição de uma função do Azure AD e $expand na função herdada de</span><span class="sxs-lookup"><span data-stu-id="e5223-174">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="e5223-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-175">Request</span></span>

<span data-ttu-id="e5223-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5223-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5223-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5223-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="e5223-178">C#</span><span class="sxs-lookup"><span data-stu-id="e5223-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5223-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5223-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5223-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5223-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5223-181">Java</span><span class="sxs-lookup"><span data-stu-id="e5223-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="e5223-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-182">Response</span></span>

<span data-ttu-id="e5223-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5223-183">The following is an example of the response.</span></span>

> <span data-ttu-id="e5223-184">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5223-184">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="e5223-185">Exemplo 4: Obter a definição de uma função criada para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="e5223-185">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5223-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-186">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e5223-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5223-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="e5223-188">C#</span><span class="sxs-lookup"><span data-stu-id="e5223-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5223-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5223-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5223-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5223-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5223-191">Java</span><span class="sxs-lookup"><span data-stu-id="e5223-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e5223-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-192">Response</span></span>
> <span data-ttu-id="e5223-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5223-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="example-5-get-the-definition-of-a-built-in-role-for-the-entitlement-management-provider"></a><span data-ttu-id="e5223-195">Exemplo 5: Obter a definição de uma função integrado para o provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="e5223-195">Example 5: Get the definition of a built-in role for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5223-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5223-196">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_built-in_entitlementmanagement_role_unifiedroledefinition"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8
```


#### <a name="response"></a><span data-ttu-id="e5223-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5223-197">Response</span></span>
> <span data-ttu-id="e5223-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5223-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


