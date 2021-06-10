---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e as relações de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 71948e099507bf081739dbef9f4e07d43f358af9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870315"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="7d70a-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="7d70a-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="7d70a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d70a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d70a-105">Obter as propriedades e as relações de [um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="7d70a-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="7d70a-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="7d70a-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="7d70a-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="7d70a-107">cloud PC</span></span> 
- <span data-ttu-id="7d70a-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="7d70a-108">device management (Intune)</span></span>
- <span data-ttu-id="7d70a-109">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="7d70a-109">directory (Azure AD)</span></span> 

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="7d70a-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d70a-110">Permissions</span></span>

<span data-ttu-id="7d70a-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7d70a-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="7d70a-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d70a-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="7d70a-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="7d70a-113">Supported provider</span></span>      | <span data-ttu-id="7d70a-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d70a-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="7d70a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d70a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d70a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d70a-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="7d70a-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="7d70a-117">Cloud PC</span></span> | <span data-ttu-id="7d70a-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="7d70a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d70a-119">Not supported.</span></span> | <span data-ttu-id="7d70a-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="7d70a-121">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7d70a-121">Device management</span></span> | <span data-ttu-id="7d70a-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="7d70a-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d70a-123">Not supported.</span></span> | <span data-ttu-id="7d70a-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="7d70a-125">Diretório</span><span class="sxs-lookup"><span data-stu-id="7d70a-125">Directory</span></span> | <span data-ttu-id="7d70a-126">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-126">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="7d70a-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d70a-127">Not supported.</span></span>| <span data-ttu-id="7d70a-128">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d70a-128">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d70a-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d70a-129">HTTP request</span></span>

<span data-ttu-id="7d70a-130">Obter uma definição de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="7d70a-130">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="7d70a-131">Obter uma definição de função para um provedor de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="7d70a-131">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="7d70a-132">Obter uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="7d70a-132">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d70a-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d70a-133">Optional query parameters</span></span>

<span data-ttu-id="7d70a-134">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d70a-134">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="7d70a-135">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7d70a-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d70a-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-136">Request headers</span></span>

| <span data-ttu-id="7d70a-137">Nome</span><span class="sxs-lookup"><span data-stu-id="7d70a-137">Name</span></span>      |<span data-ttu-id="7d70a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d70a-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d70a-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d70a-139">Authorization</span></span> | <span data-ttu-id="7d70a-140">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="7d70a-140">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d70a-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-141">Request body</span></span>

<span data-ttu-id="7d70a-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d70a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d70a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d70a-143">Response</span></span>

<span data-ttu-id="7d70a-144">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d70a-144">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d70a-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7d70a-145">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="7d70a-146">Exemplo 1: Obter a definição de uma função personalizada para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="7d70a-146">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="7d70a-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-147">Request</span></span>

<span data-ttu-id="7d70a-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d70a-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d70a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d70a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="7d70a-150">C#</span><span class="sxs-lookup"><span data-stu-id="7d70a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d70a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d70a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d70a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d70a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d70a-153">Java</span><span class="sxs-lookup"><span data-stu-id="7d70a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d70a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d70a-154">Response</span></span>

<span data-ttu-id="7d70a-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d70a-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7d70a-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d70a-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="7d70a-157">Exemplo 2: Obter a definição de uma função embutida para um provedor de diretórios</span><span class="sxs-lookup"><span data-stu-id="7d70a-157">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="7d70a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-158">Request</span></span>

<span data-ttu-id="7d70a-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d70a-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d70a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d70a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="7d70a-161">C#</span><span class="sxs-lookup"><span data-stu-id="7d70a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d70a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d70a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d70a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d70a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d70a-164">Java</span><span class="sxs-lookup"><span data-stu-id="7d70a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="7d70a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d70a-165">Response</span></span>

<span data-ttu-id="7d70a-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d70a-166">The following is an example of the response.</span></span>

> <span data-ttu-id="7d70a-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d70a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="7d70a-168">Exemplo 3: Obter a definição de uma função do Azure AD e $expand na função herdada de</span><span class="sxs-lookup"><span data-stu-id="7d70a-168">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="7d70a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-169">Request</span></span>

<span data-ttu-id="7d70a-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d70a-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d70a-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d70a-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="7d70a-172">C#</span><span class="sxs-lookup"><span data-stu-id="7d70a-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d70a-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d70a-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d70a-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d70a-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d70a-175">Java</span><span class="sxs-lookup"><span data-stu-id="7d70a-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="7d70a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d70a-176">Response</span></span>

<span data-ttu-id="7d70a-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d70a-177">The following is an example of the response.</span></span>

> <span data-ttu-id="7d70a-178">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d70a-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="7d70a-179">Exemplo 4: Obter a definição de uma função criada para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="7d70a-179">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="7d70a-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d70a-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7d70a-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d70a-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="7d70a-182">C#</span><span class="sxs-lookup"><span data-stu-id="7d70a-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d70a-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d70a-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d70a-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d70a-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d70a-185">Java</span><span class="sxs-lookup"><span data-stu-id="7d70a-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="7d70a-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d70a-186">Response</span></span>
> <span data-ttu-id="7d70a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d70a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


