---
title: Criar unifiedRoleAssignmentMultiple
description: Criar um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 326f58cdce239c2a33ac555497f67b0bc0387b71
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038517"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="be62f-103">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="be62f-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="be62f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be62f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be62f-105">Criar um novo objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="be62f-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="be62f-106">Use este objeto para criar atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="be62f-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="be62f-107">Para outros aplicativos do Micrsoft 365 (como o Azure AD), use o [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="be62f-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="be62f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="be62f-108">Permissions</span></span>

<span data-ttu-id="be62f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be62f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be62f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be62f-111">Permission type</span></span> | <span data-ttu-id="be62f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be62f-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="be62f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be62f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="be62f-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be62f-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="be62f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be62f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be62f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be62f-116">Not supported.</span></span> |
| <span data-ttu-id="be62f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be62f-117">Application</span></span> | <span data-ttu-id="be62f-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be62f-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be62f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be62f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="be62f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be62f-120">Request headers</span></span>

| <span data-ttu-id="be62f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="be62f-121">Name</span></span> | <span data-ttu-id="be62f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="be62f-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="be62f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be62f-123">Authorization</span></span> | <span data-ttu-id="be62f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be62f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="be62f-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="be62f-126">Content-type</span></span> | <span data-ttu-id="be62f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be62f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be62f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be62f-129">Request body</span></span>

<span data-ttu-id="be62f-130">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="be62f-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="be62f-131">A solicitação deve ter um escopo definido no Azure AD, como `directoryScopeIds` , ou um escopo específico de aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="be62f-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="be62f-132">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="be62f-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="be62f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="be62f-133">Response</span></span>

<span data-ttu-id="be62f-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be62f-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be62f-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be62f-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="be62f-136">Exemplo 1: criar uma atribuição de função no Intune em dois grupos de escopo (que são objetos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="be62f-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="be62f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be62f-137">Request</span></span>

<span data-ttu-id="be62f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be62f-138">The following is an example of the request.</span></span> <span data-ttu-id="be62f-139">Observe o uso do **roleTemplateId** para **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="be62f-139">Note the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="be62f-140">**roleDefinitionId** pode ser a ID de modelo de todo o serviço ou o **roleDefinitionId**específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="be62f-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="be62f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="be62f-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="be62f-142">C#</span><span class="sxs-lookup"><span data-stu-id="be62f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be62f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be62f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be62f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be62f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be62f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="be62f-145">Response</span></span>

<span data-ttu-id="be62f-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be62f-146">The following is an example of the response.</span></span>
> <span data-ttu-id="be62f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be62f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="be62f-149">Exemplo 2: criar uma atribuição de função no Intune no escopo específico do Intune de "todos os dispositivos"</span><span class="sxs-lookup"><span data-stu-id="be62f-149">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="be62f-150">Use as informações a seguir para criar atribuições de função do Intune:</span><span class="sxs-lookup"><span data-stu-id="be62f-150">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="be62f-151">Para permitir atribuições sobre todos os dispositivos do Intune, use o `AllDevices` valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="be62f-151">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="be62f-152">Para permitir atribuições sobre todos os usuários licenciados do Intune, use o `AllLicensedUsers` valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="be62f-152">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="be62f-153">Para permitir atribuições em todos os dispositivos do Intune e usuários licenciados, use o `/` valor em **directoryScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="be62f-153">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="be62f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be62f-154">Request</span></span>

<span data-ttu-id="be62f-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be62f-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="be62f-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="be62f-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="be62f-157">C#</span><span class="sxs-lookup"><span data-stu-id="be62f-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be62f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be62f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be62f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be62f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be62f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="be62f-160">Response</span></span>

<span data-ttu-id="be62f-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be62f-161">The following is an example of the response.</span></span>
> <span data-ttu-id="be62f-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be62f-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
