---
title: Criar unifiedRoleAssignmentMultiple
description: Crie um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cabca41e1935f4a17073e512ea5835d56c982643
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054739"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="ff48a-103">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ff48a-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="ff48a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff48a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff48a-105">Crie um novo [objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="ff48a-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="ff48a-106">Use este objeto para criar atribuições de função em Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="ff48a-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="ff48a-107">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff48a-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff48a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff48a-108">Permissions</span></span>

<span data-ttu-id="ff48a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff48a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ff48a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff48a-111">Permission type</span></span> | <span data-ttu-id="ff48a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff48a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="ff48a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff48a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ff48a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff48a-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="ff48a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff48a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff48a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff48a-116">Not supported.</span></span> |
| <span data-ttu-id="ff48a-117">Application</span><span class="sxs-lookup"><span data-stu-id="ff48a-117">Application</span></span> | <span data-ttu-id="ff48a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff48a-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff48a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff48a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ff48a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff48a-120">Request headers</span></span>

| <span data-ttu-id="ff48a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ff48a-121">Name</span></span> | <span data-ttu-id="ff48a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff48a-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ff48a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff48a-123">Authorization</span></span> | <span data-ttu-id="ff48a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff48a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff48a-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff48a-126">Content-type</span></span> | <span data-ttu-id="ff48a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff48a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff48a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff48a-129">Request body</span></span>

<span data-ttu-id="ff48a-130">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="ff48a-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="ff48a-131">A solicitação deve ter um escopo definido no Azure AD, como , ou um `directoryScopeIds` escopo específico do aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="ff48a-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="ff48a-132">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ff48a-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="ff48a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff48a-133">Response</span></span>

<span data-ttu-id="ff48a-134">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff48a-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ff48a-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ff48a-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="ff48a-136">Exemplo 1: Criar uma atribuição de função no Intune sobre dois grupos de escopo (que são objetos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ff48a-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="ff48a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff48a-137">Request</span></span>

<span data-ttu-id="ff48a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff48a-138">The following is an example of the request.</span></span>
> <span data-ttu-id="ff48a-139">**Observação:** o uso do **roleTemplateId** para **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="ff48a-139">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="ff48a-140">**roleDefinitionId** pode ser a ID do modelo de todo o serviço ou a função específica do **diretórioDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="ff48a-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff48a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff48a-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff48a-142">C#</span><span class="sxs-lookup"><span data-stu-id="ff48a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff48a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff48a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff48a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff48a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff48a-145">Java</span><span class="sxs-lookup"><span data-stu-id="ff48a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff48a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff48a-146">Response</span></span>

<span data-ttu-id="ff48a-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff48a-147">The following is an example of the response.</span></span>
> <span data-ttu-id="ff48a-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff48a-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="ff48a-149">Exemplo 2: Criar uma atribuição de função no Intune no escopo específico do Intune de "todos os dispositivos"</span><span class="sxs-lookup"><span data-stu-id="ff48a-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="ff48a-150">Use as seguintes informações para criar atribuições de função do Intune:</span><span class="sxs-lookup"><span data-stu-id="ff48a-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="ff48a-151">Para permitir atribuições em todos os dispositivos Intune, use `AllDevices` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="ff48a-151">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="ff48a-152">Para permitir atribuições sobre todos os usuários licenciados do Intune, use `AllLicensedUsers` o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="ff48a-152">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="ff48a-153">Para permitir atribuições em todos os dispositivos do Intune e usuários licenciados, use o `/` valor em **directoryScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="ff48a-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="ff48a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff48a-154">Request</span></span>

<span data-ttu-id="ff48a-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff48a-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff48a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff48a-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff48a-157">C#</span><span class="sxs-lookup"><span data-stu-id="ff48a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff48a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff48a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff48a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff48a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff48a-160">Java</span><span class="sxs-lookup"><span data-stu-id="ff48a-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ff48a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff48a-161">Response</span></span>

<span data-ttu-id="ff48a-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ff48a-162">The following is an example of the response.</span></span>
> <span data-ttu-id="ff48a-163">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ff48a-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


