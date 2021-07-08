---
title: Criar unifiedRoleDefinition
description: Crie um novo objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8b5fb362456b306b8f7887ad84fe80677e3262b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334609"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="a510b-103">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a510b-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="a510b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a510b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a510b-105">Crie um novo [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="a510b-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="a510b-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="a510b-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="a510b-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="a510b-107">device management (Intune)</span></span>
- <span data-ttu-id="a510b-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="a510b-108">directory (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="a510b-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="a510b-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="a510b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a510b-110">Permissions</span></span>

<span data-ttu-id="a510b-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a510b-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="a510b-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a510b-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="a510b-113">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="a510b-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="a510b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a510b-114">Permission type</span></span>      | <span data-ttu-id="a510b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a510b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a510b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a510b-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="a510b-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a510b-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="a510b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a510b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a510b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a510b-119">Not supported.</span></span>    |
|<span data-ttu-id="a510b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a510b-120">Application</span></span> | <span data-ttu-id="a510b-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a510b-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="a510b-122">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="a510b-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="a510b-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a510b-123">Permission type</span></span>      | <span data-ttu-id="a510b-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a510b-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a510b-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a510b-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="a510b-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a510b-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="a510b-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a510b-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a510b-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a510b-128">Not supported.</span></span>    |
|<span data-ttu-id="a510b-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a510b-129">Application</span></span> | <span data-ttu-id="a510b-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a510b-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a510b-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a510b-131">HTTP request</span></span>

<span data-ttu-id="a510b-132">Para criar uma definição de função para um provedor de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="a510b-132">To create a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="a510b-133">Para criar uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="a510b-133">To create a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a510b-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a510b-134">Request headers</span></span>

| <span data-ttu-id="a510b-135">Nome</span><span class="sxs-lookup"><span data-stu-id="a510b-135">Name</span></span>          | <span data-ttu-id="a510b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a510b-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a510b-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="a510b-137">Authorization</span></span> | <span data-ttu-id="a510b-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a510b-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a510b-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a510b-139">Request body</span></span>

<span data-ttu-id="a510b-140">No corpo da solicitação, fornece uma representação JSON do [objeto unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a510b-140">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="a510b-141">A tabela a seguir mostra as propriedades que são necessárias ao criar uma roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="a510b-141">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="a510b-142">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a510b-142">Parameter</span></span> | <span data-ttu-id="a510b-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="a510b-143">Type</span></span> | <span data-ttu-id="a510b-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="a510b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a510b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a510b-145">displayName</span></span> |<span data-ttu-id="a510b-146">string</span><span class="sxs-lookup"><span data-stu-id="a510b-146">string</span></span> |<span data-ttu-id="a510b-147">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a510b-147">The display name for the role definition.</span></span>|
|<span data-ttu-id="a510b-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a510b-148">isEnabled</span></span> |<span data-ttu-id="a510b-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="a510b-149">Boolean</span></span> |<span data-ttu-id="a510b-150">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a510b-150">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="a510b-151">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a510b-151">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="a510b-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a510b-152">rolePermissions</span></span> |<span data-ttu-id="a510b-153">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a510b-153">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="a510b-154">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="a510b-154">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="a510b-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a510b-155">Response</span></span>

<span data-ttu-id="a510b-156">Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a510b-156">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a510b-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a510b-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a510b-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a510b-158">Request</span></span>

<span data-ttu-id="a510b-159">A seguir, um exemplo de criação de uma função personalizada para um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="a510b-159">The following is an example of creating a custom role for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="a510b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a510b-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a510b-161">C#</span><span class="sxs-lookup"><span data-stu-id="a510b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a510b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a510b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a510b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a510b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a510b-164">Java</span><span class="sxs-lookup"><span data-stu-id="a510b-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a510b-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a510b-165">Response</span></span>

<span data-ttu-id="a510b-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a510b-166">The following is an example of the response.</span></span>
> <span data-ttu-id="a510b-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a510b-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


