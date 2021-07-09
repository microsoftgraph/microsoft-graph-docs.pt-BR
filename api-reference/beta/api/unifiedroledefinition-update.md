---
title: Atualizar unifiedRoleDefinition
description: Atualize as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: af8e75ca0364a269168c2c3b072c8c7ec6c087ae
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351073"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="1b404-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1b404-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="1b404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b404-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b404-105">Atualize as propriedades de [um objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="1b404-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="1b404-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="1b404-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="1b404-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="1b404-107">device management (Intune)</span></span>
- <span data-ttu-id="1b404-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="1b404-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="1b404-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="1b404-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b404-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b404-110">Permissions</span></span>

<span data-ttu-id="1b404-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1b404-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="1b404-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, pesquise as seguintes permissões na referência [Permissões.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="1b404-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="1b404-113">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="1b404-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="1b404-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b404-114">Permission type</span></span>      | <span data-ttu-id="1b404-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b404-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b404-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b404-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="1b404-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b404-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="1b404-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b404-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b404-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b404-119">Not supported.</span></span>    |
|<span data-ttu-id="1b404-120">Application</span><span class="sxs-lookup"><span data-stu-id="1b404-120">Application</span></span> | <span data-ttu-id="1b404-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b404-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="1b404-122">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="1b404-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="1b404-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b404-123">Permission type</span></span>      | <span data-ttu-id="1b404-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b404-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b404-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b404-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="1b404-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b404-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="1b404-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b404-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b404-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b404-128">Not supported.</span></span>    |
|<span data-ttu-id="1b404-129">Application</span><span class="sxs-lookup"><span data-stu-id="1b404-129">Application</span></span> | <span data-ttu-id="1b404-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b404-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b404-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b404-131">HTTP request</span></span>

<span data-ttu-id="1b404-132">Para atualizar uma definição de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="1b404-132">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="1b404-133">Para atualizar uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="1b404-133">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b404-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-134">Request headers</span></span>

| <span data-ttu-id="1b404-135">Nome</span><span class="sxs-lookup"><span data-stu-id="1b404-135">Name</span></span>       | <span data-ttu-id="1b404-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b404-136">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1b404-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b404-137">Authorization</span></span> | <span data-ttu-id="1b404-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1b404-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b404-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-139">Request body</span></span>

<span data-ttu-id="1b404-140">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1b404-140">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1b404-141">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1b404-141">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1b404-142">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1b404-142">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1b404-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b404-143">Property</span></span>     | <span data-ttu-id="1b404-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b404-144">Type</span></span>        | <span data-ttu-id="1b404-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b404-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b404-146">description</span><span class="sxs-lookup"><span data-stu-id="1b404-146">description</span></span>|<span data-ttu-id="1b404-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-147">String</span></span>| <span data-ttu-id="1b404-148">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="1b404-148">The description for the role definition.</span></span> <span data-ttu-id="1b404-149">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-149">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b404-150">displayName</span><span class="sxs-lookup"><span data-stu-id="1b404-150">displayName</span></span>|<span data-ttu-id="1b404-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-151">String</span></span>| <span data-ttu-id="1b404-152">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="1b404-152">The display name for the role definition.</span></span> <span data-ttu-id="1b404-153">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-153">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b404-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b404-154">Required.</span></span>|
|<span data-ttu-id="1b404-155">id</span><span class="sxs-lookup"><span data-stu-id="1b404-155">id</span></span>|<span data-ttu-id="1b404-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-156">String</span></span>| <span data-ttu-id="1b404-157">O identificador exclusivo para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="1b404-157">The unique identifier for the role definition.</span></span> <span data-ttu-id="1b404-158">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b404-158">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="1b404-159">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1b404-159">isBuiltIn</span></span>|<span data-ttu-id="1b404-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b404-160">Boolean</span></span>| <span data-ttu-id="1b404-161">Sinalizador indicando se a definição de função faz parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="1b404-161">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="1b404-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b404-162">Read-only.</span></span> |
|<span data-ttu-id="1b404-163">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1b404-163">isEnabled</span></span>|<span data-ttu-id="1b404-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b404-164">Boolean</span></span>| <span data-ttu-id="1b404-165">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="1b404-165">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="1b404-166">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="1b404-166">If false the role is not available for assignment.</span></span> <span data-ttu-id="1b404-167">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b404-168">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1b404-168">resourceScopes</span></span>|<span data-ttu-id="1b404-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-169">String collection</span></span>| <span data-ttu-id="1b404-170">Lista de permissões de escopo concedidas pela definição de função a que se aplicam.</span><span class="sxs-lookup"><span data-stu-id="1b404-170">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="1b404-171">Atualmente, apenas "/" é suportado.</span><span class="sxs-lookup"><span data-stu-id="1b404-171">Currently only "/" is supported.</span></span> <span data-ttu-id="1b404-172">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-172">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b404-173">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="1b404-173">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="1b404-174">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1b404-174">rolePermissions</span></span>|<span data-ttu-id="1b404-175">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="1b404-175">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="1b404-176">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="1b404-176">List of permissions included in the role.</span></span> <span data-ttu-id="1b404-177">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-177">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="1b404-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b404-178">Required.</span></span> |
|<span data-ttu-id="1b404-179">templateId</span><span class="sxs-lookup"><span data-stu-id="1b404-179">templateId</span></span>|<span data-ttu-id="1b404-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b404-180">String</span></span>| <span data-ttu-id="1b404-181">Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false.</span><span class="sxs-lookup"><span data-stu-id="1b404-181">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="1b404-182">Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes.</span><span class="sxs-lookup"><span data-stu-id="1b404-182">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="1b404-183">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-183">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="1b404-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="1b404-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="1b404-185">[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b404-185">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="1b404-186">Coleção somente leitura de definições de função que a definição de função determinada herda.</span><span class="sxs-lookup"><span data-stu-id="1b404-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="1b404-187">Somente funções do Azure AD integrados suportam esse atributo.</span><span class="sxs-lookup"><span data-stu-id="1b404-187">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="1b404-188">versão</span><span class="sxs-lookup"><span data-stu-id="1b404-188">version</span></span>|<span data-ttu-id="1b404-189">String</span><span class="sxs-lookup"><span data-stu-id="1b404-189">String</span></span>| <span data-ttu-id="1b404-190">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="1b404-190">Indicates version of the role definition.</span></span> <span data-ttu-id="1b404-191">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="1b404-191">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="1b404-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b404-192">Response</span></span>

<span data-ttu-id="1b404-193">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b404-193">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b404-194">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b404-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b404-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b404-195">Request</span></span>

<span data-ttu-id="1b404-196">O exemplo a seguir atualiza **um unifiedRoleDefinition** para um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="1b404-196">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b404-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b404-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="1b404-198">C#</span><span class="sxs-lookup"><span data-stu-id="1b404-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b404-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b404-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b404-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b404-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b404-201">Java</span><span class="sxs-lookup"><span data-stu-id="1b404-201">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b404-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b404-202">Response</span></span>

<span data-ttu-id="1b404-203">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b404-203">The following is an example of the response.</span></span>
> <span data-ttu-id="1b404-204">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b404-204">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


