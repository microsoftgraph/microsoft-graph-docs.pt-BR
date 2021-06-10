---
title: Criar unifiedRoleAssignmentMultiple
description: Crie um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bc09a9c514ab504d81f65983791ae947db313267
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868956"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="e80bc-103">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e80bc-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e80bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e80bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e80bc-105">Crie um novo [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="e80bc-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object for an RBAC provider.</span></span> 

<span data-ttu-id="e80bc-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="e80bc-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e80bc-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="e80bc-107">cloud PC</span></span> 
- <span data-ttu-id="e80bc-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="e80bc-108">device management (Intune)</span></span>

<span data-ttu-id="e80bc-109">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e80bc-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e80bc-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="e80bc-110">Permissions</span></span>

<span data-ttu-id="e80bc-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e80bc-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e80bc-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e80bc-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="e80bc-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="e80bc-113">Supported provider</span></span>      | <span data-ttu-id="e80bc-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e80bc-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="e80bc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e80bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e80bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e80bc-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="e80bc-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="e80bc-117">Cloud PC</span></span> | <span data-ttu-id="e80bc-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="e80bc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e80bc-119">Not supported.</span></span> | <span data-ttu-id="e80bc-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="e80bc-121">Intune</span><span class="sxs-lookup"><span data-stu-id="e80bc-121">Intune</span></span> | <span data-ttu-id="e80bc-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="e80bc-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e80bc-123">Not supported.</span></span>| <span data-ttu-id="e80bc-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e80bc-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e80bc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e80bc-125">HTTP request</span></span>

<span data-ttu-id="e80bc-126">Para criar atribuição de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="e80bc-126">To create role assignment for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="e80bc-127">Para criar atribuição de função para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="e80bc-127">To create role assignment for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e80bc-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e80bc-128">Request headers</span></span>

| <span data-ttu-id="e80bc-129">Nome</span><span class="sxs-lookup"><span data-stu-id="e80bc-129">Name</span></span> | <span data-ttu-id="e80bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80bc-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e80bc-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="e80bc-131">Authorization</span></span> | <span data-ttu-id="e80bc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e80bc-134">Content-type</span><span class="sxs-lookup"><span data-stu-id="e80bc-134">Content-type</span></span> | <span data-ttu-id="e80bc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80bc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e80bc-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e80bc-137">Request body</span></span>

<span data-ttu-id="e80bc-138">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="e80bc-138">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="e80bc-139">A solicitação deve ter um escopo definido no Azure AD, como , ou um `directoryScopeIds` escopo específico do aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="e80bc-139">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="e80bc-140">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e80bc-140">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="e80bc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80bc-141">Response</span></span>

<span data-ttu-id="e80bc-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e80bc-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e80bc-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e80bc-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="e80bc-144">Exemplo 1: Criar uma atribuição de função no Intune sobre dois grupos de escopo (que são objetos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="e80bc-144">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="e80bc-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e80bc-145">Request</span></span>

<span data-ttu-id="e80bc-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e80bc-146">The following is an example of the request.</span></span>
> <span data-ttu-id="e80bc-147">**Observação:** o uso do **roleTemplateId** para **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-147">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="e80bc-148">**roleDefinitionId** pode ser a ID do modelo de todo o serviço ou a função específica do **diretórioDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-148">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="e80bc-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e80bc-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="e80bc-150">C#</span><span class="sxs-lookup"><span data-stu-id="e80bc-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e80bc-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e80bc-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e80bc-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e80bc-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e80bc-153">Java</span><span class="sxs-lookup"><span data-stu-id="e80bc-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e80bc-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80bc-154">Response</span></span>

<span data-ttu-id="e80bc-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e80bc-155">The following is an example of the response.</span></span>
> <span data-ttu-id="e80bc-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e80bc-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="e80bc-157">Exemplo 2: Criar uma atribuição de função no Intune no escopo específico do Intune de "todos os dispositivos"</span><span class="sxs-lookup"><span data-stu-id="e80bc-157">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="e80bc-158">Use as seguintes informações para criar atribuições de função do Intune:</span><span class="sxs-lookup"><span data-stu-id="e80bc-158">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="e80bc-159">Para permitir atribuições em todos os dispositivos Intune, use `AllDevices` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-159">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="e80bc-160">Para permitir atribuições sobre todos os usuários licenciados do Intune, use `AllLicensedUsers` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-160">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="e80bc-161">Para permitir atribuições em todos os dispositivos do Intune e usuários licenciados, use o `/` valor em **directoryScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="e80bc-161">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="e80bc-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e80bc-162">Request</span></span>

<span data-ttu-id="e80bc-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e80bc-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e80bc-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="e80bc-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="e80bc-165">C#</span><span class="sxs-lookup"><span data-stu-id="e80bc-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e80bc-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e80bc-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e80bc-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e80bc-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e80bc-168">Java</span><span class="sxs-lookup"><span data-stu-id="e80bc-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e80bc-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80bc-169">Response</span></span>

<span data-ttu-id="e80bc-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e80bc-170">The following is an example of the response.</span></span>
> <span data-ttu-id="e80bc-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e80bc-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a><span data-ttu-id="e80bc-172">Exemplo 3: Criar uma atribuição de função para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="e80bc-172">Example 3: Create a role assignment for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="e80bc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e80bc-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e80bc-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="e80bc-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"]
}
```
# <a name="c"></a>[<span data-ttu-id="e80bc-175">C#</span><span class="sxs-lookup"><span data-stu-id="e80bc-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e80bc-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e80bc-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e80bc-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e80bc-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e80bc-178">Java</span><span class="sxs-lookup"><span data-stu-id="e80bc-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="e80bc-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="e80bc-179">Response</span></span>

<span data-ttu-id="e80bc-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e80bc-180">The following is an example of the response.</span></span>
> <span data-ttu-id="e80bc-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e80bc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "47c88dcd-cc79-4b0c-ba7d-7af2199649c5",
    "displayName": "My role assignment",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


