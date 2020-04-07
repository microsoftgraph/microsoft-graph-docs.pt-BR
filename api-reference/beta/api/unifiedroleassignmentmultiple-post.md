---
title: Criar unifiedRoleAssignmentMultiple
description: Criar um novo objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4238dc202068390095296b9532316cb18e6fd768
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160325"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="8c447-103">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="8c447-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="8c447-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c447-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c447-105">Criar um novo objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="8c447-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="8c447-106">Use este objeto para criar atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8c447-106">Use this object to create role assignments in Microsoft Intune.</span></span> <span data-ttu-id="8c447-107">Para outros aplicativos do Micrsoft 365 (como o Azure AD), use o [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8c447-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c447-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c447-108">Permissions</span></span>

<span data-ttu-id="8c447-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c447-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c447-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c447-111">Permission type</span></span> | <span data-ttu-id="8c447-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c447-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="8c447-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c447-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c447-114">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8c447-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="8c447-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c447-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c447-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c447-116">Not supported.</span></span> |
| <span data-ttu-id="8c447-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c447-117">Application</span></span> | <span data-ttu-id="8c447-118">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8c447-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c447-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c447-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="8c447-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c447-120">Request headers</span></span>

| <span data-ttu-id="8c447-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8c447-121">Name</span></span> | <span data-ttu-id="8c447-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c447-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="8c447-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c447-123">Authorization</span></span> | <span data-ttu-id="8c447-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c447-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c447-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="8c447-126">Content-type</span></span> | <span data-ttu-id="8c447-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c447-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c447-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c447-129">Request body</span></span>

<span data-ttu-id="8c447-130">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="8c447-130">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="8c447-131">A solicitação deve ter um escopo definido no Azure AD, como `directoryScopeIds`, ou um escopo específico de aplicativo, como. `appScopeId`</span><span class="sxs-lookup"><span data-stu-id="8c447-131">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="8c447-132">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8c447-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="8c447-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c447-133">Response</span></span>

<span data-ttu-id="8c447-134">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c447-134">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c447-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c447-135">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="8c447-136">Exemplo 1: criar uma atribuição de função no Intune em dois grupos de escopo (que são objetos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="8c447-136">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="8c447-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c447-137">Request</span></span>

<span data-ttu-id="8c447-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c447-138">The following is an example of the request.</span></span> <span data-ttu-id="8c447-139">Observe o uso do **roleTemplateId** para **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="8c447-139">Note the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="8c447-140">**roleDefinitionId** pode ser a ID de modelo de todo o serviço ou o **roleDefinitionId**específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="8c447-140">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```

#### <a name="response"></a><span data-ttu-id="8c447-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c447-141">Response</span></span>

<span data-ttu-id="8c447-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c447-142">The following is an example of the response.</span></span>
> <span data-ttu-id="8c447-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c447-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="8c447-145">Exemplo 2: criar uma atribuição de função no Intune no escopo específico do Intune de "todos os dispositivos"</span><span class="sxs-lookup"><span data-stu-id="8c447-145">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="8c447-146">Use as informações a seguir para criar atribuições de função do Intune:</span><span class="sxs-lookup"><span data-stu-id="8c447-146">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="8c447-147">Para permitir atribuições sobre todos os dispositivos do Intune `allDevices` , use o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="8c447-147">To allow assignments over all Intune devices, use the `allDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="8c447-148">Para permitir atribuições sobre todos os usuários licenciados do `allLicensedUsers` Intune, use o valor em **appScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="8c447-148">To allow assignments over all Intune licensed users, use the `allLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="8c447-149">Para permitir atribuições em todos os dispositivos do Intune e usuários licenciados, use o `/` valor em **directoryScopeIds**.</span><span class="sxs-lookup"><span data-stu-id="8c447-149">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="8c447-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c447-150">Request</span></span>

<span data-ttu-id="8c447-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c447-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

#### <a name="response"></a><span data-ttu-id="8c447-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c447-152">Response</span></span>

<span data-ttu-id="8c447-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8c447-153">The following is an example of the response.</span></span>
> <span data-ttu-id="8c447-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c447-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
