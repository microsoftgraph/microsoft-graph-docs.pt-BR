---
title: Criar unifiedRoleAssignment
description: Crie um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aafcc34d288dcce1bcd0970802472a2e2e565e83
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317200"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="9a0d6-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9a0d6-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="9a0d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a0d6-105">Crie um novo [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9a0d6-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a0d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a0d6-106">Permissions</span></span>

<span data-ttu-id="9a0d6-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="9a0d6-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a0d6-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0d6-109">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="9a0d6-109">Supported provider</span></span>      | <span data-ttu-id="9a0d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a0d6-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="9a0d6-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a0d6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a0d6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a0d6-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="9a0d6-113">Diretório</span><span class="sxs-lookup"><span data-stu-id="9a0d6-113">Directory</span></span> | <span data-ttu-id="9a0d6-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9a0d6-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="9a0d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-115">Not supported.</span></span>| <span data-ttu-id="9a0d6-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9a0d6-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="9a0d6-117">Gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="9a0d6-117">Entitlement management</span></span> | <span data-ttu-id="9a0d6-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0d6-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="9a0d6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-119">Not supported.</span></span> | <span data-ttu-id="9a0d6-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a0d6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0d6-121">HTTP request</span></span>

<span data-ttu-id="9a0d6-122">Crie uma atribuição de função para o provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="9a0d6-122">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="9a0d6-123">Crie uma atribuição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="9a0d6-123">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="9a0d6-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0d6-124">Request headers</span></span>

| <span data-ttu-id="9a0d6-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9a0d6-125">Name</span></span>          | <span data-ttu-id="9a0d6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a0d6-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9a0d6-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a0d6-127">Authorization</span></span> | <span data-ttu-id="9a0d6-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9a0d6-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a0d6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0d6-129">Request body</span></span>

<span data-ttu-id="9a0d6-130">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9a0d6-130">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="9a0d6-131">A solicitação deve ter um escopo definido no Azure AD, como , ou um `directoryScopeId` escopo específico do aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="9a0d6-131">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="9a0d6-132">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="9a0d6-133">Para obter mais informações, consulte [appScope](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="9a0d6-133">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="9a0d6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0d6-134">Response</span></span>

<span data-ttu-id="9a0d6-135">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-135">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a0d6-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a0d6-136">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="9a0d6-137">Exemplo 1: Criar uma atribuição de função no escopo do locatário</span><span class="sxs-lookup"><span data-stu-id="9a0d6-137">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="9a0d6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0d6-138">Request</span></span>

<span data-ttu-id="9a0d6-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-139">The following is an example of the request.</span></span> <span data-ttu-id="9a0d6-140">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-140">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="9a0d6-141">roleDefinitionId pode ser a ID do modelo de todo o serviço ou a função específica do diretórioDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-141">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a0d6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0d6-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9a0d6-143">C#</span><span class="sxs-lookup"><span data-stu-id="9a0d6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a0d6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a0d6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a0d6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a0d6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a0d6-146">Java</span><span class="sxs-lookup"><span data-stu-id="9a0d6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a0d6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0d6-147">Response</span></span>

<span data-ttu-id="9a0d6-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-148">The following is an example of the response.</span></span>

> <span data-ttu-id="9a0d6-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="9a0d6-150">Exemplo 2: Criar uma atribuição de função em um escopo de unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="9a0d6-150">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="9a0d6-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0d6-151">Request</span></span>

<span data-ttu-id="9a0d6-152">O exemplo a seguir atribui uma função de Administrador de Usuário principal sobre uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-152">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a0d6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0d6-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9a0d6-154">C#</span><span class="sxs-lookup"><span data-stu-id="9a0d6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a0d6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a0d6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a0d6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a0d6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a0d6-157">Java</span><span class="sxs-lookup"><span data-stu-id="9a0d6-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9a0d6-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0d6-158">Response</span></span>

<span data-ttu-id="9a0d6-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-159">The following is an example of the response.</span></span>

> <span data-ttu-id="9a0d6-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a0d6-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


