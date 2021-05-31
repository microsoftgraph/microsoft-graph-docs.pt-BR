---
title: Criar unifiedRoleDefinition
description: Crie um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e5512205b346d1005b8ce51f3ab11afa4f95a9a2
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709501"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="8d951-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8d951-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="8d951-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d951-105">Crie um novo [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="8d951-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="8d951-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="8d951-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="8d951-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="8d951-107">device management (Intune)</span></span>
- <span data-ttu-id="8d951-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="8d951-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="8d951-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="8d951-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d951-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d951-110">Permissions</span></span>

<span data-ttu-id="8d951-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8d951-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="8d951-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d951-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="8d951-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="8d951-113">Supported provider</span></span>      | <span data-ttu-id="8d951-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d951-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="8d951-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d951-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d951-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d951-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="8d951-117">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="8d951-117">Device management</span></span> | <span data-ttu-id="8d951-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d951-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="8d951-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d951-119">Not supported.</span></span> | <span data-ttu-id="8d951-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d951-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="8d951-121">Diretório</span><span class="sxs-lookup"><span data-stu-id="8d951-121">Directory</span></span> | <span data-ttu-id="8d951-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d951-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="8d951-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d951-123">Not supported.</span></span>| <span data-ttu-id="8d951-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d951-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d951-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d951-125">HTTP request</span></span>

<span data-ttu-id="8d951-126">Para criar uma definição de função para um provedor de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="8d951-126">To create a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="8d951-127">Para criar uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="8d951-127">To create a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8d951-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d951-128">Request headers</span></span>

| <span data-ttu-id="8d951-129">Nome</span><span class="sxs-lookup"><span data-stu-id="8d951-129">Name</span></span>          | <span data-ttu-id="8d951-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d951-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d951-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d951-131">Authorization</span></span> | <span data-ttu-id="8d951-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8d951-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d951-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d951-133">Request body</span></span>

<span data-ttu-id="8d951-134">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d951-134">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="8d951-135">A tabela a seguir mostra as propriedades que são necessárias ao criar uma roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d951-135">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="8d951-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d951-136">Parameter</span></span> | <span data-ttu-id="8d951-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d951-137">Type</span></span> | <span data-ttu-id="8d951-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d951-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d951-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8d951-139">displayName</span></span> |<span data-ttu-id="8d951-140">string</span><span class="sxs-lookup"><span data-stu-id="8d951-140">string</span></span> |<span data-ttu-id="8d951-141">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="8d951-141">The display name for the role definition.</span></span>|
|<span data-ttu-id="8d951-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8d951-142">isEnabled</span></span> |<span data-ttu-id="8d951-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d951-143">Boolean</span></span> |<span data-ttu-id="8d951-144">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="8d951-144">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="8d951-145">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="8d951-145">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="8d951-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8d951-146">rolePermissions</span></span> |<span data-ttu-id="8d951-147">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8d951-147">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="8d951-148">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="8d951-148">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="8d951-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d951-149">Response</span></span>

<span data-ttu-id="8d951-150">Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d951-150">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d951-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d951-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d951-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d951-152">Request</span></span>

<span data-ttu-id="8d951-153">A seguir, um exemplo de criação de uma função personalizada para um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="8d951-153">The following is an example of creating a custom role for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d951-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d951-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d951-155">C#</span><span class="sxs-lookup"><span data-stu-id="8d951-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d951-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d951-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d951-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d951-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d951-158">Java</span><span class="sxs-lookup"><span data-stu-id="8d951-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d951-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d951-159">Response</span></span>

<span data-ttu-id="8d951-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d951-160">The following is an example of the response.</span></span>
> <span data-ttu-id="8d951-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d951-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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


