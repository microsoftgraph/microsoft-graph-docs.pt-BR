---
title: Criar unifiedRoleAssignmentMultiple
description: Crie um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9883ea3666b22ddaa21de349b56e361a02d99396
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334602"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="33b7d-103">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="33b7d-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="33b7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33b7d-105">Crie um novo [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="33b7d-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object for an RBAC provider.</span></span> 

<span data-ttu-id="33b7d-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="33b7d-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="33b7d-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="33b7d-107">cloud PC</span></span> 
- <span data-ttu-id="33b7d-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="33b7d-108">device management (Intune)</span></span>

<span data-ttu-id="33b7d-109">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="33b7d-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="33b7d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="33b7d-110">Permissions</span></span>

<span data-ttu-id="33b7d-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="33b7d-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="33b7d-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33b7d-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="33b7d-113">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="33b7d-113">For Cloud PC provider</span></span>

|<span data-ttu-id="33b7d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b7d-114">Permission type</span></span>      | <span data-ttu-id="33b7d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33b7d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b7d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b7d-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="33b7d-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b7d-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="33b7d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b7d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b7d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b7d-119">Not supported.</span></span>    |
|<span data-ttu-id="33b7d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b7d-120">Application</span></span> | <span data-ttu-id="33b7d-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b7d-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="33b7d-122">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="33b7d-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="33b7d-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33b7d-123">Permission type</span></span>      | <span data-ttu-id="33b7d-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33b7d-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b7d-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33b7d-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="33b7d-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b7d-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="33b7d-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33b7d-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b7d-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33b7d-128">Not supported.</span></span>    |
|<span data-ttu-id="33b7d-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33b7d-129">Application</span></span> | <span data-ttu-id="33b7d-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33b7d-130">DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="33b7d-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33b7d-131">HTTP request</span></span>

<span data-ttu-id="33b7d-132">Para criar atribuição de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="33b7d-132">To create role assignment for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="33b7d-133">Para criar atribuição de função para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="33b7d-133">To create role assignment for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="33b7d-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33b7d-134">Request headers</span></span>

| <span data-ttu-id="33b7d-135">Nome</span><span class="sxs-lookup"><span data-stu-id="33b7d-135">Name</span></span> | <span data-ttu-id="33b7d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b7d-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="33b7d-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="33b7d-137">Authorization</span></span> | <span data-ttu-id="33b7d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b7d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33b7d-140">Content-type</span><span class="sxs-lookup"><span data-stu-id="33b7d-140">Content-type</span></span> | <span data-ttu-id="33b7d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33b7d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33b7d-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33b7d-143">Request body</span></span>

<span data-ttu-id="33b7d-144">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="33b7d-144">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="33b7d-145">A solicitação deve ter um escopo definido no Azure AD, como , ou um `directoryScopeIds` escopo específico do aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="33b7d-145">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="33b7d-146">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="33b7d-146">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="33b7d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b7d-147">Response</span></span>

<span data-ttu-id="33b7d-148">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33b7d-148">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33b7d-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="33b7d-149">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="33b7d-150">Exemplo 1: Criar uma atribuição de função no Intune sobre dois grupos de escopo (que são objetos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="33b7d-150">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="33b7d-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b7d-151">Request</span></span>

<span data-ttu-id="33b7d-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b7d-152">The following is an example of the request.</span></span>
> <span data-ttu-id="33b7d-153">**Observação:** o uso do **roleTemplateId** para **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="33b7d-153">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="33b7d-154">**roleDefinitionId** pode ser a ID do modelo de todo o serviço ou a função específica do **diretórioDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="33b7d-154">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="33b7d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="33b7d-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33b7d-156">C#</span><span class="sxs-lookup"><span data-stu-id="33b7d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33b7d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33b7d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33b7d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33b7d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33b7d-159">Java</span><span class="sxs-lookup"><span data-stu-id="33b7d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33b7d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b7d-160">Response</span></span>

<span data-ttu-id="33b7d-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33b7d-161">The following is an example of the response.</span></span>
> <span data-ttu-id="33b7d-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33b7d-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="33b7d-163">Exemplo 2: Criar uma atribuição de função no Intune no escopo específico do Intune de "todos os dispositivos"</span><span class="sxs-lookup"><span data-stu-id="33b7d-163">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="33b7d-164">Use as seguintes informações para criar atribuições de função do Intune:</span><span class="sxs-lookup"><span data-stu-id="33b7d-164">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="33b7d-165">Para permitir atribuições em todos os dispositivos Intune, use `AllDevices` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="33b7d-165">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="33b7d-166">Para permitir atribuições sobre todos os usuários licenciados do Intune, use `AllLicensedUsers` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="33b7d-166">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="33b7d-167">Para permitir atribuições em todos os dispositivos do Intune e usuários licenciados, use o `/` valor em **directoryScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="33b7d-167">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="33b7d-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b7d-168">Request</span></span>

<span data-ttu-id="33b7d-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33b7d-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="33b7d-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="33b7d-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33b7d-171">C#</span><span class="sxs-lookup"><span data-stu-id="33b7d-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33b7d-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33b7d-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33b7d-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33b7d-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33b7d-174">Java</span><span class="sxs-lookup"><span data-stu-id="33b7d-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="33b7d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b7d-175">Response</span></span>

<span data-ttu-id="33b7d-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33b7d-176">The following is an example of the response.</span></span>
> <span data-ttu-id="33b7d-177">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="33b7d-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a><span data-ttu-id="33b7d-178">Exemplo 3: Criar uma atribuição de função para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="33b7d-178">Example 3: Create a role assignment for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="33b7d-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33b7d-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="33b7d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="33b7d-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="33b7d-181">C#</span><span class="sxs-lookup"><span data-stu-id="33b7d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33b7d-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33b7d-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33b7d-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33b7d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33b7d-184">Java</span><span class="sxs-lookup"><span data-stu-id="33b7d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="33b7d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="33b7d-185">Response</span></span>

<span data-ttu-id="33b7d-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33b7d-186">The following is an example of the response.</span></span>
> <span data-ttu-id="33b7d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33b7d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


