---
title: Criar unifiedRoleAssignment
description: Crie um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a7587bf4dea653b86b4f93632e5719bcec4aaaaa
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351101"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="81b1a-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="81b1a-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="81b1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b1a-105">Crie um novo [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81b1a-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81b1a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81b1a-106">Permissions</span></span>

<span data-ttu-id="81b1a-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="81b1a-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="81b1a-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81b1a-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="81b1a-109">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="81b1a-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="81b1a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81b1a-110">Permission type</span></span>      | <span data-ttu-id="81b1a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81b1a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81b1a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81b1a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="81b1a-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81b1a-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="81b1a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81b1a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81b1a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b1a-115">Not supported.</span></span>    |
|<span data-ttu-id="81b1a-116">Application</span><span class="sxs-lookup"><span data-stu-id="81b1a-116">Application</span></span> | <span data-ttu-id="81b1a-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81b1a-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="81b1a-118">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="81b1a-118">For Entitlement management provider</span></span>

|<span data-ttu-id="81b1a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81b1a-119">Permission type</span></span>      | <span data-ttu-id="81b1a-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81b1a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81b1a-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81b1a-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="81b1a-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b1a-122">EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="81b1a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81b1a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81b1a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b1a-124">Not supported.</span></span>    |
|<span data-ttu-id="81b1a-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b1a-125">Application</span></span> | <span data-ttu-id="81b1a-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b1a-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81b1a-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81b1a-127">HTTP request</span></span>

<span data-ttu-id="81b1a-128">Crie uma atribuição de função para o provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="81b1a-128">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="81b1a-129">Crie uma atribuição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="81b1a-129">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="81b1a-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81b1a-130">Request headers</span></span>

| <span data-ttu-id="81b1a-131">Nome</span><span class="sxs-lookup"><span data-stu-id="81b1a-131">Name</span></span>          | <span data-ttu-id="81b1a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b1a-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81b1a-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="81b1a-133">Authorization</span></span> | <span data-ttu-id="81b1a-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="81b1a-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="81b1a-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81b1a-135">Request body</span></span>

<span data-ttu-id="81b1a-136">No corpo da solicitação, fornece uma representação JSON de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81b1a-136">In the request body, supply a JSON representation of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="81b1a-137">A solicitação deve ter um escopo definido no Azure AD, como **directoryScopeId** ou um escopo específico do aplicativo, como **appScopeId**.</span><span class="sxs-lookup"><span data-stu-id="81b1a-137">The request must have either a scope defined in Azure AD, such as **directoryScopeId**, or an application-specific scope, such as **appScopeId**.</span></span> <span data-ttu-id="81b1a-138">Exemplos de escopos do Azure AD são locatário ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="81b1a-138">Examples of Azure AD scopes are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="81b1a-139">O gerenciamento de direitos usa escopos de catálogo de pacotes de locatários ("/") e de acesso.</span><span class="sxs-lookup"><span data-stu-id="81b1a-139">Entitlement management uses tenant ("/") and access package catalog scopes.</span></span> <span data-ttu-id="81b1a-140">Para obter mais informações, consulte [appScope](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="81b1a-140">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="81b1a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b1a-141">Response</span></span>

<span data-ttu-id="81b1a-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81b1a-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81b1a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81b1a-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="81b1a-144">Exemplo 1: Criar uma atribuição de função no escopo do locatário</span><span class="sxs-lookup"><span data-stu-id="81b1a-144">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="81b1a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b1a-145">Request</span></span>

<span data-ttu-id="81b1a-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b1a-146">The following is an example of the request.</span></span> <span data-ttu-id="81b1a-147">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="81b1a-147">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="81b1a-148">roleDefinitionId pode ser a ID do modelo de todo o serviço ou a função específica do diretórioDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="81b1a-148">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="81b1a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="81b1a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```
# <a name="c"></a>[<span data-ttu-id="81b1a-150">C#</span><span class="sxs-lookup"><span data-stu-id="81b1a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81b1a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81b1a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81b1a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81b1a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81b1a-153">Java</span><span class="sxs-lookup"><span data-stu-id="81b1a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81b1a-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b1a-154">Response</span></span>

<span data-ttu-id="81b1a-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81b1a-155">The following is an example of the response.</span></span>

> <span data-ttu-id="81b1a-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81b1a-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="81b1a-157">Exemplo 2: Criar uma atribuição de função em um escopo de unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="81b1a-157">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="81b1a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b1a-158">Request</span></span>

<span data-ttu-id="81b1a-159">O exemplo a seguir atribui uma função de Administrador de Usuário principal sobre uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="81b1a-159">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="81b1a-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="81b1a-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_over_administrativeunit"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1", //template id of User Account Administrator
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[<span data-ttu-id="81b1a-161">C#</span><span class="sxs-lookup"><span data-stu-id="81b1a-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81b1a-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81b1a-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81b1a-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81b1a-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81b1a-164">Java</span><span class="sxs-lookup"><span data-stu-id="81b1a-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81b1a-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b1a-165">Response</span></span>

<span data-ttu-id="81b1a-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81b1a-166">The following is an example of the response.</span></span>

> <span data-ttu-id="81b1a-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81b1a-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "BH21sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHIWb7-1",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
}
```


### <a name="example-3-create-a-role-assignment-at-access-package-catalog-scope"></a><span data-ttu-id="81b1a-168">Exemplo 3: Criar uma atribuição de função no escopo do catálogo de pacotes de acesso</span><span class="sxs-lookup"><span data-stu-id="81b1a-168">Example 3: Create a role assignment at access package catalog scope</span></span>

#### <a name="request"></a><span data-ttu-id="81b1a-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b1a-169">Request</span></span>

<span data-ttu-id="81b1a-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b1a-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment3_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleAssignments
Content-type: application/json

{
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```

#### <a name="response"></a><span data-ttu-id="81b1a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b1a-171">Response</span></span>

<span data-ttu-id="81b1a-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81b1a-172">The following is an example of the response.</span></span>

> <span data-ttu-id="81b1a-173">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81b1a-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleAssignments/$entity",
    "id": "f3092518-7874-462e-93e9-0cd6c11ffc52",
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

