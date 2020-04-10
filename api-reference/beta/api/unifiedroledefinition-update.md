---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb1cd8a7e8cbef279c5007b3cd721193ff25e518
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218938"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="ac367-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ac367-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="ac367-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac367-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac367-105">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ac367-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac367-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac367-106">Permissions</span></span>

<span data-ttu-id="ac367-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac367-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac367-109">Permission type</span></span>                        | <span data-ttu-id="ac367-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac367-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac367-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac367-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac367-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="ac367-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="ac367-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac367-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac367-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac367-114">Not supported.</span></span> |
| <span data-ttu-id="ac367-115">Application</span><span class="sxs-lookup"><span data-stu-id="ac367-115">Application</span></span>                            | <span data-ttu-id="ac367-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="ac367-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac367-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac367-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ac367-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac367-118">Request headers</span></span>

| <span data-ttu-id="ac367-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ac367-119">Name</span></span>       | <span data-ttu-id="ac367-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac367-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac367-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac367-121">Authorization</span></span> | <span data-ttu-id="ac367-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ac367-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac367-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac367-123">Request body</span></span>

<span data-ttu-id="ac367-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ac367-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ac367-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ac367-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ac367-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ac367-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac367-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac367-127">Property</span></span>     | <span data-ttu-id="ac367-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac367-128">Type</span></span>        | <span data-ttu-id="ac367-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac367-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac367-130">description</span><span class="sxs-lookup"><span data-stu-id="ac367-130">description</span></span>|<span data-ttu-id="ac367-131">String</span><span class="sxs-lookup"><span data-stu-id="ac367-131">String</span></span>| <span data-ttu-id="ac367-132">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ac367-132">The description for the role definition.</span></span> <span data-ttu-id="ac367-133">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ac367-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ac367-134">displayName</span></span>|<span data-ttu-id="ac367-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac367-135">String</span></span>| <span data-ttu-id="ac367-136">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ac367-136">The display name for the role definition.</span></span> <span data-ttu-id="ac367-137">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ac367-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac367-138">Required.</span></span>|
|<span data-ttu-id="ac367-139">id</span><span class="sxs-lookup"><span data-stu-id="ac367-139">id</span></span>|<span data-ttu-id="ac367-140">String</span><span class="sxs-lookup"><span data-stu-id="ac367-140">String</span></span>| <span data-ttu-id="ac367-141">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ac367-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="ac367-142">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac367-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="ac367-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ac367-143">isBuiltIn</span></span>|<span data-ttu-id="ac367-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac367-144">Boolean</span></span>| <span data-ttu-id="ac367-145">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="ac367-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="ac367-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac367-146">Read-only.</span></span> |
|<span data-ttu-id="ac367-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ac367-147">isEnabled</span></span>|<span data-ttu-id="ac367-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac367-148">Boolean</span></span>| <span data-ttu-id="ac367-149">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ac367-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="ac367-150">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ac367-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="ac367-151">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ac367-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ac367-152">resourceScopes</span></span>|<span data-ttu-id="ac367-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac367-153">String collection</span></span>| <span data-ttu-id="ac367-154">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="ac367-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="ac367-155">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="ac367-155">Currently only "/" is supported.</span></span> <span data-ttu-id="ac367-156">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ac367-157">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="ac367-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="ac367-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ac367-158">rolePermissions</span></span>|<span data-ttu-id="ac367-159">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ac367-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="ac367-160">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="ac367-160">List of permissions included in the role.</span></span> <span data-ttu-id="ac367-161">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ac367-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac367-162">Required.</span></span> |
|<span data-ttu-id="ac367-163">templateId</span><span class="sxs-lookup"><span data-stu-id="ac367-163">templateId</span></span>|<span data-ttu-id="ac367-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ac367-164">String</span></span>| <span data-ttu-id="ac367-165">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="ac367-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="ac367-166">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="ac367-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="ac367-167">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ac367-168">versão</span><span class="sxs-lookup"><span data-stu-id="ac367-168">version</span></span>|<span data-ttu-id="ac367-169">String</span><span class="sxs-lookup"><span data-stu-id="ac367-169">String</span></span>| <span data-ttu-id="ac367-170">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ac367-170">Indicates version of the role definition.</span></span> <span data-ttu-id="ac367-171">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ac367-171">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="ac367-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac367-172">Response</span></span>

<span data-ttu-id="ac367-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac367-173">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac367-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac367-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac367-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac367-175">Request</span></span>

<span data-ttu-id="ac367-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac367-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ac367-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac367-177">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac367-178">C#</span><span class="sxs-lookup"><span data-stu-id="ac367-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac367-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac367-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac367-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac367-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac367-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac367-181">Response</span></span>

<span data-ttu-id="ac367-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac367-182">The following is an example of the response.</span></span>
> <span data-ttu-id="ac367-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac367-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
