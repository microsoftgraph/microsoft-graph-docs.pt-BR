---
title: Atualizar unifiedRoleDefinition
description: Atualize as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47ff9ff4c40360ddb28d5d6d344ca1d7375cc119
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709490"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="6401e-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6401e-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="6401e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6401e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6401e-105">Atualize as propriedades de [um objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="6401e-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="6401e-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="6401e-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="6401e-107">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="6401e-107">device management (Intune)</span></span>
- <span data-ttu-id="6401e-108">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="6401e-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="6401e-109">No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="6401e-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="6401e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6401e-110">Permissions</span></span>

<span data-ttu-id="6401e-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6401e-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="6401e-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6401e-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="6401e-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="6401e-113">Supported provider</span></span>      | <span data-ttu-id="6401e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6401e-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="6401e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6401e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6401e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6401e-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="6401e-117">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="6401e-117">Device management</span></span> | <span data-ttu-id="6401e-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6401e-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="6401e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6401e-119">Not supported.</span></span> | <span data-ttu-id="6401e-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6401e-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="6401e-121">Diretório</span><span class="sxs-lookup"><span data-stu-id="6401e-121">Directory</span></span> | <span data-ttu-id="6401e-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6401e-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="6401e-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6401e-123">Not supported.</span></span>| <span data-ttu-id="6401e-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6401e-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6401e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6401e-125">HTTP request</span></span>

<span data-ttu-id="6401e-126">Para atualizar uma definição de função para um provedor de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="6401e-126">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="6401e-127">Para atualizar uma definição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="6401e-127">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6401e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6401e-128">Request headers</span></span>

| <span data-ttu-id="6401e-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6401e-129">Name</span></span>       | <span data-ttu-id="6401e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6401e-130">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6401e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="6401e-131">Authorization</span></span> | <span data-ttu-id="6401e-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6401e-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6401e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6401e-133">Request body</span></span>

<span data-ttu-id="6401e-134">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6401e-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6401e-135">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6401e-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6401e-136">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6401e-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6401e-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6401e-137">Property</span></span>     | <span data-ttu-id="6401e-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="6401e-138">Type</span></span>        | <span data-ttu-id="6401e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6401e-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6401e-140">description</span><span class="sxs-lookup"><span data-stu-id="6401e-140">description</span></span>|<span data-ttu-id="6401e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6401e-141">String</span></span>| <span data-ttu-id="6401e-142">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="6401e-142">The description for the role definition.</span></span> <span data-ttu-id="6401e-143">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-143">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="6401e-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6401e-144">displayName</span></span>|<span data-ttu-id="6401e-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6401e-145">String</span></span>| <span data-ttu-id="6401e-146">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="6401e-146">The display name for the role definition.</span></span> <span data-ttu-id="6401e-147">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-147">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="6401e-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6401e-148">Required.</span></span>|
|<span data-ttu-id="6401e-149">id</span><span class="sxs-lookup"><span data-stu-id="6401e-149">id</span></span>|<span data-ttu-id="6401e-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6401e-150">String</span></span>| <span data-ttu-id="6401e-151">O identificador exclusivo para a definição de função.</span><span class="sxs-lookup"><span data-stu-id="6401e-151">The unique identifier for the role definition.</span></span> <span data-ttu-id="6401e-152">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6401e-152">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="6401e-153">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="6401e-153">isBuiltIn</span></span>|<span data-ttu-id="6401e-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="6401e-154">Boolean</span></span>| <span data-ttu-id="6401e-155">Sinalizador indicando se a definição de função faz parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="6401e-155">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="6401e-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6401e-156">Read-only.</span></span> |
|<span data-ttu-id="6401e-157">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6401e-157">isEnabled</span></span>|<span data-ttu-id="6401e-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="6401e-158">Boolean</span></span>| <span data-ttu-id="6401e-159">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="6401e-159">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="6401e-160">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="6401e-160">If false the role is not available for assignment.</span></span> <span data-ttu-id="6401e-161">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="6401e-162">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6401e-162">resourceScopes</span></span>|<span data-ttu-id="6401e-163">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6401e-163">String collection</span></span>| <span data-ttu-id="6401e-164">Lista de permissões de escopo concedidas pela definição de função a que se aplicam.</span><span class="sxs-lookup"><span data-stu-id="6401e-164">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="6401e-165">Atualmente, apenas "/" é suportado.</span><span class="sxs-lookup"><span data-stu-id="6401e-165">Currently only "/" is supported.</span></span> <span data-ttu-id="6401e-166">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-166">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="6401e-167">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="6401e-167">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="6401e-168">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="6401e-168">rolePermissions</span></span>|<span data-ttu-id="6401e-169">[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="6401e-169">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="6401e-170">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="6401e-170">List of permissions included in the role.</span></span> <span data-ttu-id="6401e-171">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-171">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="6401e-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6401e-172">Required.</span></span> |
|<span data-ttu-id="6401e-173">templateId</span><span class="sxs-lookup"><span data-stu-id="6401e-173">templateId</span></span>|<span data-ttu-id="6401e-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6401e-174">String</span></span>| <span data-ttu-id="6401e-175">Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false.</span><span class="sxs-lookup"><span data-stu-id="6401e-175">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="6401e-176">Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes.</span><span class="sxs-lookup"><span data-stu-id="6401e-176">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="6401e-177">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-177">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="6401e-178">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="6401e-178">inheritsPermissionsFrom</span></span>| <span data-ttu-id="6401e-179">[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6401e-179">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="6401e-180">Coleção somente leitura de definições de função que a definição de função determinada herda.</span><span class="sxs-lookup"><span data-stu-id="6401e-180">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="6401e-181">Somente funções do Azure AD integrados suportam esse atributo.</span><span class="sxs-lookup"><span data-stu-id="6401e-181">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="6401e-182">versão</span><span class="sxs-lookup"><span data-stu-id="6401e-182">version</span></span>|<span data-ttu-id="6401e-183">String</span><span class="sxs-lookup"><span data-stu-id="6401e-183">String</span></span>| <span data-ttu-id="6401e-184">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="6401e-184">Indicates version of the role definition.</span></span> <span data-ttu-id="6401e-185">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="6401e-185">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="6401e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="6401e-186">Response</span></span>

<span data-ttu-id="6401e-187">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6401e-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6401e-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6401e-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="6401e-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6401e-189">Request</span></span>

<span data-ttu-id="6401e-190">O exemplo a seguir atualiza **um unifiedRoleDefinition** para um provedor de diretórios.</span><span class="sxs-lookup"><span data-stu-id="6401e-190">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="6401e-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="6401e-191">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6401e-192">C#</span><span class="sxs-lookup"><span data-stu-id="6401e-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6401e-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6401e-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6401e-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6401e-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6401e-195">Java</span><span class="sxs-lookup"><span data-stu-id="6401e-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6401e-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="6401e-196">Response</span></span>

<span data-ttu-id="6401e-197">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6401e-197">The following is an example of the response.</span></span>
> <span data-ttu-id="6401e-198">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6401e-198">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
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


