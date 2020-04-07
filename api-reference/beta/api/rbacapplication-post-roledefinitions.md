---
title: Criar unifiedRoleDefinition
description: Criar um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38105a80378ad38fc931abb2e0a94eac0d8a517d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160244"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="284b8-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="284b8-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="284b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="284b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="284b8-105">Criar um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="284b8-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="284b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="284b8-106">Permissions</span></span>

<span data-ttu-id="284b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="284b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="284b8-109">Permission type</span></span>                        | <span data-ttu-id="284b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="284b8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="284b8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="284b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="284b8-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="284b8-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="284b8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="284b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="284b8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="284b8-114">Not supported.</span></span> |
| <span data-ttu-id="284b8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="284b8-115">Application</span></span>                            | <span data-ttu-id="284b8-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="284b8-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="284b8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="284b8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="284b8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="284b8-118">Request headers</span></span>

| <span data-ttu-id="284b8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="284b8-119">Name</span></span>          | <span data-ttu-id="284b8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="284b8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="284b8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="284b8-121">Authorization</span></span> | <span data-ttu-id="284b8-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="284b8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="284b8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="284b8-123">Request body</span></span>

<span data-ttu-id="284b8-124">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="284b8-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="284b8-125">A tabela a seguir mostra as propriedades que são necessárias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="284b8-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="284b8-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="284b8-126">Parameter</span></span> | <span data-ttu-id="284b8-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="284b8-127">Type</span></span> | <span data-ttu-id="284b8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="284b8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="284b8-129">displayName</span><span class="sxs-lookup"><span data-stu-id="284b8-129">displayName</span></span> |<span data-ttu-id="284b8-130">string</span><span class="sxs-lookup"><span data-stu-id="284b8-130">string</span></span> |<span data-ttu-id="284b8-131">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="284b8-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="284b8-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="284b8-132">isEnabled</span></span> |<span data-ttu-id="284b8-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="284b8-133">Boolean</span></span> |<span data-ttu-id="284b8-134">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="284b8-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="284b8-135">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="284b8-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="284b8-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="284b8-136">rolePermissions</span></span> |<span data-ttu-id="284b8-137">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="284b8-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="284b8-138">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="284b8-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="284b8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="284b8-139">Response</span></span>

<span data-ttu-id="284b8-140">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="284b8-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="284b8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="284b8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="284b8-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="284b8-142">Request</span></span>

<span data-ttu-id="284b8-143">Veja a seguir um exemplo de criação de uma função personalizada.</span><span class="sxs-lookup"><span data-stu-id="284b8-143">The following is an example of creating a custom role.</span></span>

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

### <a name="response"></a><span data-ttu-id="284b8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="284b8-144">Response</span></span>

<span data-ttu-id="284b8-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="284b8-145">The following is an example of the response.</span></span>
> <span data-ttu-id="284b8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="284b8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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