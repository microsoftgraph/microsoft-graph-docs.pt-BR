---
title: Criar unifiedRoleAssignment
description: Crie um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d654b852358c94e4b762c794c6da114f19b091af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440882"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="1dc15-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1dc15-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="1dc15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dc15-105">Crie um novo [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1dc15-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dc15-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dc15-106">Permissions</span></span>

<span data-ttu-id="1dc15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dc15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dc15-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dc15-109">Permission type</span></span>                        | <span data-ttu-id="1dc15-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dc15-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1dc15-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dc15-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dc15-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="1dc15-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="1dc15-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dc15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dc15-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dc15-114">Not supported.</span></span> |
| <span data-ttu-id="1dc15-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dc15-115">Application</span></span>                            | <span data-ttu-id="1dc15-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="1dc15-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dc15-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="1dc15-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc15-118">Request headers</span></span>

| <span data-ttu-id="1dc15-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1dc15-119">Name</span></span>          | <span data-ttu-id="1dc15-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc15-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1dc15-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dc15-121">Authorization</span></span> | <span data-ttu-id="1dc15-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1dc15-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dc15-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc15-123">Request body</span></span>

<span data-ttu-id="1dc15-124">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1dc15-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="1dc15-125">A solicitação deve ter um escopo definido no Azure AD, como , ou um `directoryScopeId` escopo específico do aplicativo, como `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="1dc15-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="1dc15-126">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1dc15-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="1dc15-127">Para obter mais informações, consulte [appScope](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="1dc15-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="1dc15-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc15-128">Response</span></span>

<span data-ttu-id="1dc15-129">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc15-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dc15-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1dc15-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="1dc15-131">Exemplo 1: Criar uma atribuição de função no escopo do locatário</span><span class="sxs-lookup"><span data-stu-id="1dc15-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="1dc15-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc15-132">Request</span></span>

<span data-ttu-id="1dc15-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dc15-133">The following is an example of the request.</span></span> <span data-ttu-id="1dc15-134">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="1dc15-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="1dc15-135">roleDefinitionId pode ser a ID do modelo de todo o serviço ou a função específica do diretórioDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="1dc15-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="1dc15-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc15-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dc15-137">C#</span><span class="sxs-lookup"><span data-stu-id="1dc15-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dc15-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dc15-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dc15-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dc15-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dc15-140">Java</span><span class="sxs-lookup"><span data-stu-id="1dc15-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1dc15-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc15-141">Response</span></span>

<span data-ttu-id="1dc15-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc15-142">The following is an example of the response.</span></span>

> <span data-ttu-id="1dc15-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dc15-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="1dc15-145">Exemplo 2: Criar uma atribuição de função em um escopo de unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="1dc15-145">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="1dc15-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc15-146">Request</span></span>

<span data-ttu-id="1dc15-147">O exemplo a seguir atribui uma função de Administrador de Usuário principal sobre uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="1dc15-147">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="1dc15-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc15-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1dc15-149">C#</span><span class="sxs-lookup"><span data-stu-id="1dc15-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dc15-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dc15-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dc15-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dc15-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dc15-152">Java</span><span class="sxs-lookup"><span data-stu-id="1dc15-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1dc15-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc15-153">Response</span></span>

<span data-ttu-id="1dc15-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc15-154">The following is an example of the response.</span></span>

> <span data-ttu-id="1dc15-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dc15-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


