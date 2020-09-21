---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: afb8dbdb19816b487dfe7fe60cd09897120caa2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968980"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="dd922-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="dd922-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="dd922-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd922-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd922-105">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="dd922-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd922-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd922-106">Permissions</span></span>

<span data-ttu-id="dd922-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd922-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd922-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd922-109">Permission type</span></span>                        | <span data-ttu-id="dd922-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd922-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd922-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd922-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd922-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="dd922-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="dd922-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd922-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd922-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd922-114">Not supported.</span></span> |
| <span data-ttu-id="dd922-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd922-115">Application</span></span>                            | <span data-ttu-id="dd922-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="dd922-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd922-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd922-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd922-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd922-118">Request headers</span></span>

| <span data-ttu-id="dd922-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dd922-119">Name</span></span>       | <span data-ttu-id="dd922-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd922-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dd922-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd922-121">Authorization</span></span> | <span data-ttu-id="dd922-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dd922-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd922-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd922-123">Request body</span></span>

<span data-ttu-id="dd922-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="dd922-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="dd922-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="dd922-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dd922-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dd922-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd922-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd922-127">Property</span></span>     | <span data-ttu-id="dd922-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd922-128">Type</span></span>        | <span data-ttu-id="dd922-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd922-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd922-130">description</span><span class="sxs-lookup"><span data-stu-id="dd922-130">description</span></span>|<span data-ttu-id="dd922-131">String</span><span class="sxs-lookup"><span data-stu-id="dd922-131">String</span></span>| <span data-ttu-id="dd922-132">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="dd922-132">The description for the role definition.</span></span> <span data-ttu-id="dd922-133">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd922-134">displayName</span><span class="sxs-lookup"><span data-stu-id="dd922-134">displayName</span></span>|<span data-ttu-id="dd922-135">String</span><span class="sxs-lookup"><span data-stu-id="dd922-135">String</span></span>| <span data-ttu-id="dd922-136">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="dd922-136">The display name for the role definition.</span></span> <span data-ttu-id="dd922-137">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="dd922-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd922-138">Required.</span></span>|
|<span data-ttu-id="dd922-139">id</span><span class="sxs-lookup"><span data-stu-id="dd922-139">id</span></span>|<span data-ttu-id="dd922-140">String</span><span class="sxs-lookup"><span data-stu-id="dd922-140">String</span></span>| <span data-ttu-id="dd922-141">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="dd922-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="dd922-142">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd922-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="dd922-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="dd922-143">isBuiltIn</span></span>|<span data-ttu-id="dd922-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd922-144">Boolean</span></span>| <span data-ttu-id="dd922-145">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="dd922-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="dd922-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd922-146">Read-only.</span></span> |
|<span data-ttu-id="dd922-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="dd922-147">isEnabled</span></span>|<span data-ttu-id="dd922-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd922-148">Boolean</span></span>| <span data-ttu-id="dd922-149">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="dd922-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="dd922-150">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="dd922-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="dd922-151">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd922-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="dd922-152">resourceScopes</span></span>|<span data-ttu-id="dd922-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd922-153">String collection</span></span>| <span data-ttu-id="dd922-154">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="dd922-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="dd922-155">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="dd922-155">Currently only "/" is supported.</span></span> <span data-ttu-id="dd922-156">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="dd922-157">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="dd922-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="dd922-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="dd922-158">rolePermissions</span></span>|<span data-ttu-id="dd922-159">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dd922-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="dd922-160">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="dd922-160">List of permissions included in the role.</span></span> <span data-ttu-id="dd922-161">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="dd922-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd922-162">Required.</span></span> |
|<span data-ttu-id="dd922-163">templateId</span><span class="sxs-lookup"><span data-stu-id="dd922-163">templateId</span></span>|<span data-ttu-id="dd922-164">String</span><span class="sxs-lookup"><span data-stu-id="dd922-164">String</span></span>| <span data-ttu-id="dd922-165">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="dd922-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="dd922-166">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="dd922-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="dd922-167">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="dd922-168">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="dd922-168">inheritsPermissionsFrom</span></span>| <span data-ttu-id="dd922-169">coleção [unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dd922-169">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="dd922-170">Coleção somente leitura de definições de função que a definição de função fornecida herda.</span><span class="sxs-lookup"><span data-stu-id="dd922-170">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="dd922-171">Somente as funções internas do Azure AD dão suporte a esse atributo.</span><span class="sxs-lookup"><span data-stu-id="dd922-171">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="dd922-172">versão</span><span class="sxs-lookup"><span data-stu-id="dd922-172">version</span></span>|<span data-ttu-id="dd922-173">String</span><span class="sxs-lookup"><span data-stu-id="dd922-173">String</span></span>| <span data-ttu-id="dd922-174">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="dd922-174">Indicates version of the role definition.</span></span> <span data-ttu-id="dd922-175">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="dd922-175">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="dd922-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd922-176">Response</span></span>

<span data-ttu-id="dd922-177">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd922-177">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd922-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd922-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd922-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd922-179">Request</span></span>

<span data-ttu-id="dd922-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd922-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd922-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd922-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dd922-182">C#</span><span class="sxs-lookup"><span data-stu-id="dd922-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd922-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd922-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd922-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd922-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd922-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd922-185">Response</span></span>

<span data-ttu-id="dd922-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd922-186">The following is an example of the response.</span></span>
> <span data-ttu-id="dd922-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd922-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


