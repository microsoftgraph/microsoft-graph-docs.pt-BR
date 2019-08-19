---
title: Criar unifiedRoleDefinition
description: Criar um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74a67f090d37fe6eff0b4910862eabafcfcd27c7
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461255"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="41729-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="41729-103">Create unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41729-104">Criar um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="41729-104">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="41729-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="41729-105">Permissions</span></span>

<span data-ttu-id="41729-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41729-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41729-108">Permission type</span></span>                        | <span data-ttu-id="41729-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41729-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41729-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41729-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41729-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="41729-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="41729-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41729-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41729-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41729-113">Not supported.</span></span> |
| <span data-ttu-id="41729-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41729-114">Application</span></span>                            | <span data-ttu-id="41729-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="41729-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="41729-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41729-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="41729-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41729-117">Request headers</span></span>

| <span data-ttu-id="41729-118">Nome</span><span class="sxs-lookup"><span data-stu-id="41729-118">Name</span></span>          | <span data-ttu-id="41729-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="41729-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="41729-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="41729-120">Authorization</span></span> | <span data-ttu-id="41729-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="41729-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41729-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41729-122">Request body</span></span>

<span data-ttu-id="41729-123">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="41729-123">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="41729-124">A tabela a seguir mostra as propriedades que são necessárias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="41729-124">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="41729-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="41729-125">Parameter</span></span> | <span data-ttu-id="41729-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="41729-126">Type</span></span> | <span data-ttu-id="41729-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="41729-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41729-128">displayName</span><span class="sxs-lookup"><span data-stu-id="41729-128">displayName</span></span> |<span data-ttu-id="41729-129">string</span><span class="sxs-lookup"><span data-stu-id="41729-129">string</span></span> |<span data-ttu-id="41729-130">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="41729-130">The display name for the role definition.</span></span>|
|<span data-ttu-id="41729-131">isEnabled</span><span class="sxs-lookup"><span data-stu-id="41729-131">isEnabled</span></span> |<span data-ttu-id="41729-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="41729-132">Boolean</span></span> |<span data-ttu-id="41729-133">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="41729-133">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="41729-134">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="41729-134">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="41729-135">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="41729-135">rolePermissions</span></span> |<span data-ttu-id="41729-136">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="41729-136">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="41729-137">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="41729-137">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="41729-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="41729-138">Response</span></span>

<span data-ttu-id="41729-139">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41729-139">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41729-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41729-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="41729-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41729-141">Request</span></span>

<span data-ttu-id="41729-142">Veja a seguir um exemplo de criação de uma função personalizada.</span><span class="sxs-lookup"><span data-stu-id="41729-142">The following is an example of creating a custom role.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41729-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="41729-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="41729-144">C#</span><span class="sxs-lookup"><span data-stu-id="41729-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41729-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41729-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41729-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="41729-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41729-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="41729-147">Response</span></span>

<span data-ttu-id="41729-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41729-148">The following is an example of the response.</span></span>

> <span data-ttu-id="41729-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41729-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "resourceScopes": [
        "/"
    ],
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
