---
title: Criar unifiedRoleAssignment
description: Criar um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12a7168b32c3ee0a246b02a4a4d72f92041227e5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160251"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="e3049-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e3049-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="e3049-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3049-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3049-105">Criar um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e3049-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3049-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3049-106">Permissions</span></span>

<span data-ttu-id="e3049-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3049-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3049-109">Permission type</span></span>                        | <span data-ttu-id="e3049-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3049-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3049-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3049-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3049-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="e3049-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="e3049-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3049-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3049-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3049-114">Not supported.</span></span> |
| <span data-ttu-id="e3049-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3049-115">Application</span></span>                            | <span data-ttu-id="e3049-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="e3049-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3049-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3049-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e3049-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3049-118">Request headers</span></span>

| <span data-ttu-id="e3049-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e3049-119">Name</span></span>          | <span data-ttu-id="e3049-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3049-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e3049-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3049-121">Authorization</span></span> | <span data-ttu-id="e3049-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e3049-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3049-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3049-123">Request body</span></span>

<span data-ttu-id="e3049-124">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e3049-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="e3049-125">A solicitação deve ter um escopo definido no Azure AD, como `directoryScopeId`, ou um escopo específico de aplicativo, como. `appScopeId`</span><span class="sxs-lookup"><span data-stu-id="e3049-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="e3049-126">Exemplos de escopo do Azure AD são locatários ("/"), unidades administrativas ou aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e3049-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="e3049-127">Para obter mais informações, consulte [appScope](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="e3049-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="e3049-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3049-128">Response</span></span>

<span data-ttu-id="e3049-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3049-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3049-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3049-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="e3049-131">Exemplo 1: criar uma atribuição de função no escopo do locatário</span><span class="sxs-lookup"><span data-stu-id="e3049-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="e3049-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3049-132">Request</span></span>

<span data-ttu-id="e3049-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3049-133">The following is an example of the request.</span></span> <span data-ttu-id="e3049-134">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="e3049-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="e3049-135">roleDefinitionId pode ser a ID de modelo de todo o serviço ou o roleDefinitionId específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="e3049-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

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

#### <a name="response"></a><span data-ttu-id="e3049-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3049-136">Response</span></span>

<span data-ttu-id="e3049-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3049-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e3049-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3049-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="e3049-140">Exemplo 2: criar uma atribuição de função em um escopo de unidade administrativa</span><span class="sxs-lookup"><span data-stu-id="e3049-140">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="e3049-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3049-141">Request</span></span>

<span data-ttu-id="e3049-142">O exemplo a seguir atribui uma função de administrador de usuário principal em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="e3049-142">The following example assigns a principal User Admin role over an administrative unit.</span></span>

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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```

#### <a name="response"></a><span data-ttu-id="e3049-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3049-143">Response</span></span>

<span data-ttu-id="e3049-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3049-144">The following is an example of the response.</span></span>

> <span data-ttu-id="e3049-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3049-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
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