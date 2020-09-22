---
title: Criar unifiedRoleAssignment
description: Criar um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac8588470d7c52bdd163567bee8a1210dd5478a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050406"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="8fed4-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8fed4-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="8fed4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fed4-105">Criar um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8fed4-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fed4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fed4-106">Permissions</span></span>

<span data-ttu-id="8fed4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8fed4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fed4-109">Permission type</span></span>                        | <span data-ttu-id="8fed4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fed4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8fed4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fed4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fed4-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="8fed4-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="8fed4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fed4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fed4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fed4-114">Not supported.</span></span> |
| <span data-ttu-id="8fed4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fed4-115">Application</span></span>                            | <span data-ttu-id="8fed4-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="8fed4-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fed4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fed4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="8fed4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fed4-118">Request headers</span></span>

| <span data-ttu-id="8fed4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8fed4-119">Name</span></span>          | <span data-ttu-id="8fed4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fed4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8fed4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fed4-121">Authorization</span></span> | <span data-ttu-id="8fed4-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8fed4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fed4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fed4-123">Request body</span></span>

<span data-ttu-id="8fed4-124">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8fed4-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="8fed4-125">A solicitação deve ter um escopo definido no Azure AD, como `directoryScopeId` , ou um escopo específico de aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="8fed4-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="8fed4-126">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8fed4-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="8fed4-127">Para obter mais informações, consulte [appScope](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="8fed4-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="8fed4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fed4-128">Response</span></span>

<span data-ttu-id="8fed4-129">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fed4-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8fed4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8fed4-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="8fed4-131">Exemplo 1: criar uma atribuição de função no escopo do locatário</span><span class="sxs-lookup"><span data-stu-id="8fed4-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="8fed4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fed4-132">Request</span></span>

<span data-ttu-id="8fed4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fed4-133">The following is an example of the request.</span></span> <span data-ttu-id="8fed4-134">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="8fed4-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="8fed4-135">roleDefinitionId pode ser a ID de modelo de todo o serviço ou o roleDefinitionId específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="8fed4-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="8fed4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fed4-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8fed4-137">C#</span><span class="sxs-lookup"><span data-stu-id="8fed4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fed4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fed4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fed4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fed4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8fed4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fed4-140">Response</span></span>

<span data-ttu-id="8fed4-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8fed4-141">The following is an example of the response.</span></span>

> <span data-ttu-id="8fed4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fed4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="8fed4-144">Exemplo 2: criar uma atribuição de função em um escopo de unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="8fed4-144">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="8fed4-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fed4-145">Request</span></span>

<span data-ttu-id="8fed4-146">O exemplo a seguir atribui uma função de administrador de usuário principal em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="8fed4-146">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="8fed4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fed4-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8fed4-148">C#</span><span class="sxs-lookup"><span data-stu-id="8fed4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fed4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fed4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fed4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fed4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8fed4-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fed4-151">Response</span></span>

<span data-ttu-id="8fed4-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8fed4-152">The following is an example of the response.</span></span>

> <span data-ttu-id="8fed4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fed4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


