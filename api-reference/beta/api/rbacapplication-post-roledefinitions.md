---
title: Criar unifiedRoleDefinition
description: Criar um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b05074aed0c8204645c96e8a5e2e8af1d00fec91
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43216726"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="a6ebb-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6ebb-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="a6ebb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6ebb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6ebb-105">Criar um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a6ebb-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6ebb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6ebb-106">Permissions</span></span>

<span data-ttu-id="a6ebb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6ebb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6ebb-109">Permission type</span></span>                        | <span data-ttu-id="a6ebb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6ebb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6ebb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6ebb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6ebb-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a6ebb-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="a6ebb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6ebb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6ebb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-114">Not supported.</span></span> |
| <span data-ttu-id="a6ebb-115">Application</span><span class="sxs-lookup"><span data-stu-id="a6ebb-115">Application</span></span>                            | <span data-ttu-id="a6ebb-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a6ebb-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6ebb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ebb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a6ebb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ebb-118">Request headers</span></span>

| <span data-ttu-id="a6ebb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a6ebb-119">Name</span></span>          | <span data-ttu-id="a6ebb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ebb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a6ebb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6ebb-121">Authorization</span></span> | <span data-ttu-id="a6ebb-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a6ebb-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6ebb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ebb-123">Request body</span></span>

<span data-ttu-id="a6ebb-124">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a6ebb-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="a6ebb-125">A tabela a seguir mostra as propriedades que são necessárias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="a6ebb-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6ebb-126">Parameter</span></span> | <span data-ttu-id="a6ebb-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6ebb-127">Type</span></span> | <span data-ttu-id="a6ebb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6ebb-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6ebb-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a6ebb-129">displayName</span></span> |<span data-ttu-id="a6ebb-130">string</span><span class="sxs-lookup"><span data-stu-id="a6ebb-130">string</span></span> |<span data-ttu-id="a6ebb-131">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="a6ebb-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a6ebb-132">isEnabled</span></span> |<span data-ttu-id="a6ebb-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6ebb-133">Boolean</span></span> |<span data-ttu-id="a6ebb-134">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="a6ebb-135">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="a6ebb-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a6ebb-136">rolePermissions</span></span> |<span data-ttu-id="a6ebb-137">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a6ebb-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="a6ebb-138">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="a6ebb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ebb-139">Response</span></span>

<span data-ttu-id="a6ebb-140">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6ebb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6ebb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6ebb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6ebb-142">Request</span></span>

<span data-ttu-id="a6ebb-143">Veja a seguir um exemplo de criação de uma função personalizada.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-143">The following is an example of creating a custom role.</span></span>


# <a name="http"></a>[<span data-ttu-id="a6ebb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ebb-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6ebb-145">C#</span><span class="sxs-lookup"><span data-stu-id="a6ebb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6ebb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6ebb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6ebb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6ebb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6ebb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6ebb-148">Response</span></span>

<span data-ttu-id="a6ebb-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-149">The following is an example of the response.</span></span>
> <span data-ttu-id="a6ebb-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6ebb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    ]
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
