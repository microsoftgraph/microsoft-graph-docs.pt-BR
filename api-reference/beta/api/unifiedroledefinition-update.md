---
title: Atualizar unifiedRoleDefinition
description: Atualize as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e5315a58adc5c6b4447b725ee7315d390d18904
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334714"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="0ce98-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ce98-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="0ce98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ce98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce98-105">Atualize as propriedades de [um objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="0ce98-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="0ce98-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="0ce98-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="0ce98-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="0ce98-107">device management (Intune)</span></span>
- <span data-ttu-id="0ce98-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="0ce98-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="0ce98-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="0ce98-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce98-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ce98-110">Permissions</span></span>

<span data-ttu-id="0ce98-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="0ce98-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="0ce98-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, pesquise as seguintes permissões na referência [Permissões.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="0ce98-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="0ce98-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="0ce98-113">Supported provider</span></span>      | <span data-ttu-id="0ce98-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ce98-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="0ce98-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ce98-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce98-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ce98-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="0ce98-117">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="0ce98-117">Device management</span></span> | <span data-ttu-id="0ce98-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="0ce98-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce98-119">Not supported.</span></span> | <span data-ttu-id="0ce98-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0ce98-121">Diretório</span><span class="sxs-lookup"><span data-stu-id="0ce98-121">Directory</span></span> | <span data-ttu-id="0ce98-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="0ce98-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce98-123">Not supported.</span></span>| <span data-ttu-id="0ce98-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="0ce98-125">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="0ce98-125">For Device management (Intune) provider</span></span>

|<span data-ttu-id="0ce98-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ce98-126">Permission type</span></span>      | <span data-ttu-id="0ce98-127">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ce98-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce98-128">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ce98-128">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ce98-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-129">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="0ce98-130">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ce98-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce98-131">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce98-131">Not supported.</span></span>    |
|<span data-ttu-id="0ce98-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ce98-132">Application</span></span> | <span data-ttu-id="0ce98-133">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-133">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="0ce98-134">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="0ce98-134">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="0ce98-135">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ce98-135">Permission type</span></span>      | <span data-ttu-id="0ce98-136">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ce98-136">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce98-137">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ce98-137">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ce98-138">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-138">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="0ce98-139">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ce98-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce98-140">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ce98-140">Not supported.</span></span>    |
|<span data-ttu-id="0ce98-141">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ce98-141">Application</span></span> | <span data-ttu-id="0ce98-142">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce98-142">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ce98-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce98-143">HTTP request</span></span>

<span data-ttu-id="0ce98-144">Para atualizar uma definição de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="0ce98-144">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="0ce98-145">Para atualizar uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="0ce98-145">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ce98-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce98-146">Request headers</span></span>

| <span data-ttu-id="0ce98-147">Nome</span><span class="sxs-lookup"><span data-stu-id="0ce98-147">Name</span></span>       | <span data-ttu-id="0ce98-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce98-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ce98-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ce98-149">Authorization</span></span> | <span data-ttu-id="0ce98-150">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0ce98-150">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ce98-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce98-151">Request body</span></span>

<span data-ttu-id="0ce98-152">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0ce98-152">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0ce98-153">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0ce98-153">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0ce98-154">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0ce98-154">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ce98-155">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ce98-155">Property</span></span>     | <span data-ttu-id="0ce98-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ce98-156">Type</span></span>        | <span data-ttu-id="0ce98-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ce98-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ce98-158">description</span><span class="sxs-lookup"><span data-stu-id="0ce98-158">description</span></span>|<span data-ttu-id="0ce98-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ce98-159">String</span></span>| <span data-ttu-id="0ce98-160">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0ce98-160">The description for the role definition.</span></span> <span data-ttu-id="0ce98-161">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0ce98-162">displayName</span><span class="sxs-lookup"><span data-stu-id="0ce98-162">displayName</span></span>|<span data-ttu-id="0ce98-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ce98-163">String</span></span>| <span data-ttu-id="0ce98-164">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0ce98-164">The display name for the role definition.</span></span> <span data-ttu-id="0ce98-165">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-165">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="0ce98-166">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ce98-166">Required.</span></span>|
|<span data-ttu-id="0ce98-167">id</span><span class="sxs-lookup"><span data-stu-id="0ce98-167">id</span></span>|<span data-ttu-id="0ce98-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ce98-168">String</span></span>| <span data-ttu-id="0ce98-169">O identificador exclusivo para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="0ce98-169">The unique identifier for the role definition.</span></span> <span data-ttu-id="0ce98-170">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ce98-170">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="0ce98-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0ce98-171">isBuiltIn</span></span>|<span data-ttu-id="0ce98-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ce98-172">Boolean</span></span>| <span data-ttu-id="0ce98-173">Sinalizador indicando se a definição de função faz parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="0ce98-173">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="0ce98-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ce98-174">Read-only.</span></span> |
|<span data-ttu-id="0ce98-175">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0ce98-175">isEnabled</span></span>|<span data-ttu-id="0ce98-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ce98-176">Boolean</span></span>| <span data-ttu-id="0ce98-177">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="0ce98-177">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="0ce98-178">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="0ce98-178">If false the role is not available for assignment.</span></span> <span data-ttu-id="0ce98-179">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-179">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0ce98-180">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0ce98-180">resourceScopes</span></span>|<span data-ttu-id="0ce98-181">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ce98-181">String collection</span></span>| <span data-ttu-id="0ce98-182">Lista de permissões de escopo concedidas pela definição de função a que se aplicam.</span><span class="sxs-lookup"><span data-stu-id="0ce98-182">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="0ce98-183">Atualmente, apenas "/" é suportado.</span><span class="sxs-lookup"><span data-stu-id="0ce98-183">Currently only "/" is supported.</span></span> <span data-ttu-id="0ce98-184">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-184">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="0ce98-185">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="0ce98-185">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="0ce98-186">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="0ce98-186">rolePermissions</span></span>|<span data-ttu-id="0ce98-187">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0ce98-187">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="0ce98-188">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="0ce98-188">List of permissions included in the role.</span></span> <span data-ttu-id="0ce98-189">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-189">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="0ce98-190">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ce98-190">Required.</span></span> |
|<span data-ttu-id="0ce98-191">templateId</span><span class="sxs-lookup"><span data-stu-id="0ce98-191">templateId</span></span>|<span data-ttu-id="0ce98-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ce98-192">String</span></span>| <span data-ttu-id="0ce98-193">Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false.</span><span class="sxs-lookup"><span data-stu-id="0ce98-193">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="0ce98-194">Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes.</span><span class="sxs-lookup"><span data-stu-id="0ce98-194">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="0ce98-195">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-195">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="0ce98-196">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="0ce98-196">inheritsPermissionsFrom</span></span>| <span data-ttu-id="0ce98-197">[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ce98-197">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="0ce98-198">Coleção somente leitura de definições de função que a definição de função determinada herda.</span><span class="sxs-lookup"><span data-stu-id="0ce98-198">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="0ce98-199">Somente funções do Azure AD integrados suportam esse atributo.</span><span class="sxs-lookup"><span data-stu-id="0ce98-199">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="0ce98-200">versão</span><span class="sxs-lookup"><span data-stu-id="0ce98-200">version</span></span>|<span data-ttu-id="0ce98-201">String</span><span class="sxs-lookup"><span data-stu-id="0ce98-201">String</span></span>| <span data-ttu-id="0ce98-202">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="0ce98-202">Indicates version of the role definition.</span></span> <span data-ttu-id="0ce98-203">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="0ce98-203">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="0ce98-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ce98-204">Response</span></span>

<span data-ttu-id="0ce98-205">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ce98-205">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ce98-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ce98-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ce98-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ce98-207">Request</span></span>

<span data-ttu-id="0ce98-208">O exemplo a seguir atualiza **um unifiedRoleDefinition** para um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="0ce98-208">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="0ce98-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce98-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ce98-210">C#</span><span class="sxs-lookup"><span data-stu-id="0ce98-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ce98-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ce98-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ce98-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ce98-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ce98-213">Java</span><span class="sxs-lookup"><span data-stu-id="0ce98-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ce98-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ce98-214">Response</span></span>

<span data-ttu-id="0ce98-215">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ce98-215">The following is an example of the response.</span></span>
> <span data-ttu-id="0ce98-216">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ce98-216">**Note:** The response object shown here might be shortened for readability.</span></span>

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


