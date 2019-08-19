---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3be16446147e3e0dd9d4c2a481b5fdae63312f6a
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461595"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="909d5-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="909d5-103">Update unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="909d5-104">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="909d5-104">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="909d5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="909d5-105">Permissions</span></span>

<span data-ttu-id="909d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="909d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="909d5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="909d5-108">Permission type</span></span>                        | <span data-ttu-id="909d5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="909d5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="909d5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="909d5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="909d5-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="909d5-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="909d5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="909d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="909d5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="909d5-113">Not supported.</span></span> |
| <span data-ttu-id="909d5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="909d5-114">Application</span></span>                            | <span data-ttu-id="909d5-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="909d5-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="909d5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="909d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="909d5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="909d5-117">Request headers</span></span>

| <span data-ttu-id="909d5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="909d5-118">Name</span></span>       | <span data-ttu-id="909d5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="909d5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="909d5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="909d5-120">Authorization</span></span> | <span data-ttu-id="909d5-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="909d5-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="909d5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="909d5-122">Request body</span></span>

<span data-ttu-id="909d5-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="909d5-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="909d5-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="909d5-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="909d5-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="909d5-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="909d5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="909d5-126">Property</span></span>     | <span data-ttu-id="909d5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="909d5-127">Type</span></span>        | <span data-ttu-id="909d5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="909d5-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="909d5-129">description</span><span class="sxs-lookup"><span data-stu-id="909d5-129">description</span></span>|<span data-ttu-id="909d5-130">String</span><span class="sxs-lookup"><span data-stu-id="909d5-130">String</span></span>| <span data-ttu-id="909d5-131">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="909d5-131">The description for the role definition.</span></span> <span data-ttu-id="909d5-132">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="909d5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="909d5-133">displayName</span></span>|<span data-ttu-id="909d5-134">String</span><span class="sxs-lookup"><span data-stu-id="909d5-134">String</span></span>| <span data-ttu-id="909d5-135">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="909d5-135">The display name for the role definition.</span></span> <span data-ttu-id="909d5-136">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="909d5-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="909d5-137">Required.</span></span>|
|<span data-ttu-id="909d5-138">id</span><span class="sxs-lookup"><span data-stu-id="909d5-138">id</span></span>|<span data-ttu-id="909d5-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="909d5-139">String</span></span>| <span data-ttu-id="909d5-140">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="909d5-140">The unique identifier for the role definition.</span></span> <span data-ttu-id="909d5-141">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="909d5-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="909d5-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="909d5-142">isBuiltIn</span></span>|<span data-ttu-id="909d5-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="909d5-143">Boolean</span></span>| <span data-ttu-id="909d5-144">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="909d5-144">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="909d5-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="909d5-145">Read-only.</span></span> |
|<span data-ttu-id="909d5-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="909d5-146">isEnabled</span></span>|<span data-ttu-id="909d5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="909d5-147">Boolean</span></span>| <span data-ttu-id="909d5-148">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="909d5-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="909d5-149">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="909d5-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="909d5-150">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="909d5-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="909d5-151">resourceScopes</span></span>|<span data-ttu-id="909d5-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="909d5-152">String collection</span></span>| <span data-ttu-id="909d5-153">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="909d5-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="909d5-154">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="909d5-154">Currently only "/" is supported.</span></span> <span data-ttu-id="909d5-155">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-155">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="909d5-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="909d5-156">rolePermissions</span></span>|<span data-ttu-id="909d5-157">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="909d5-157">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="909d5-158">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="909d5-158">List of permissions included in the role.</span></span> <span data-ttu-id="909d5-159">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-159">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="909d5-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="909d5-160">Required.</span></span> |
|<span data-ttu-id="909d5-161">templateId</span><span class="sxs-lookup"><span data-stu-id="909d5-161">templateId</span></span>|<span data-ttu-id="909d5-162">String</span><span class="sxs-lookup"><span data-stu-id="909d5-162">String</span></span>| <span data-ttu-id="909d5-163">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="909d5-163">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="909d5-164">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="909d5-164">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="909d5-165">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-165">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="909d5-166">versão</span><span class="sxs-lookup"><span data-stu-id="909d5-166">version</span></span>|<span data-ttu-id="909d5-167">String</span><span class="sxs-lookup"><span data-stu-id="909d5-167">String</span></span>| <span data-ttu-id="909d5-168">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="909d5-168">Indicates version of the role definition.</span></span> <span data-ttu-id="909d5-169">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="909d5-169">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="909d5-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="909d5-170">Response</span></span>

<span data-ttu-id="909d5-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="909d5-171">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="909d5-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="909d5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="909d5-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="909d5-173">Request</span></span>

<span data-ttu-id="909d5-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="909d5-174">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="909d5-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="909d5-175">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="909d5-176">C#</span><span class="sxs-lookup"><span data-stu-id="909d5-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="909d5-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="909d5-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="909d5-178">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="909d5-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="909d5-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="909d5-179">Response</span></span>

<span data-ttu-id="909d5-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="909d5-180">The following is an example of the response.</span></span>

> <span data-ttu-id="909d5-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="909d5-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
