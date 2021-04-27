---
title: Criar unifiedRoleDefinition
description: Crie um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 92d02320b102cedf1cef95f6966d97d78ad341d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051001"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="ea4a2-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ea4a2-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="ea4a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea4a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea4a2-105">Crie um novo [objeto unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea4a2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea4a2-106">Permissions</span></span>

<span data-ttu-id="ea4a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea4a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea4a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea4a2-109">Permission type</span></span>                        | <span data-ttu-id="ea4a2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea4a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea4a2-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="ea4a2-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="ea4a2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea4a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-114">Not supported.</span></span> |
| <span data-ttu-id="ea4a2-115">Application</span><span class="sxs-lookup"><span data-stu-id="ea4a2-115">Application</span></span>                            | <span data-ttu-id="ea4a2-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="ea4a2-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea4a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea4a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ea4a2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea4a2-118">Request headers</span></span>

| <span data-ttu-id="ea4a2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ea4a2-119">Name</span></span>          | <span data-ttu-id="ea4a2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4a2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ea4a2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea4a2-121">Authorization</span></span> | <span data-ttu-id="ea4a2-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ea4a2-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea4a2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea4a2-123">Request body</span></span>

<span data-ttu-id="ea4a2-124">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="ea4a2-125">A tabela a seguir mostra as propriedades que são necessárias ao criar uma roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="ea4a2-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ea4a2-126">Parameter</span></span> | <span data-ttu-id="ea4a2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea4a2-127">Type</span></span> | <span data-ttu-id="ea4a2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4a2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea4a2-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ea4a2-129">displayName</span></span> |<span data-ttu-id="ea4a2-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea4a2-130">string</span></span> |<span data-ttu-id="ea4a2-131">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="ea4a2-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ea4a2-132">isEnabled</span></span> |<span data-ttu-id="ea4a2-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea4a2-133">Boolean</span></span> |<span data-ttu-id="ea4a2-134">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="ea4a2-135">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="ea4a2-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ea4a2-136">rolePermissions</span></span> |<span data-ttu-id="ea4a2-137">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ea4a2-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="ea4a2-138">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="ea4a2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea4a2-139">Response</span></span>

<span data-ttu-id="ea4a2-140">Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea4a2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea4a2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea4a2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea4a2-142">Request</span></span>

<span data-ttu-id="ea4a2-143">A seguir, um exemplo de criação de uma função personalizada.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-143">The following is an example of creating a custom role.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea4a2-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea4a2-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[<span data-ttu-id="ea4a2-145">C#</span><span class="sxs-lookup"><span data-stu-id="ea4a2-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea4a2-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea4a2-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea4a2-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea4a2-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea4a2-148">Java</span><span class="sxs-lookup"><span data-stu-id="ea4a2-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea4a2-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea4a2-149">Response</span></span>

<span data-ttu-id="ea4a2-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-150">The following is an example of the response.</span></span>
> <span data-ttu-id="ea4a2-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('c2cb59a3-2d01-4176-a458-95b0e674966f')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


