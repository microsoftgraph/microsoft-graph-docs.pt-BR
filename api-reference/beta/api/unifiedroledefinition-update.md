---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee564c893473231cddf68e804b767c2f8142137a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452047"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="10a86-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10a86-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="10a86-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="10a86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10a86-105">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="10a86-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10a86-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10a86-106">Permissions</span></span>

<span data-ttu-id="10a86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10a86-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10a86-109">Permission type</span></span>                        | <span data-ttu-id="10a86-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10a86-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10a86-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10a86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10a86-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="10a86-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="10a86-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10a86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10a86-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10a86-114">Not supported.</span></span> |
| <span data-ttu-id="10a86-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10a86-115">Application</span></span>                            | <span data-ttu-id="10a86-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="10a86-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="10a86-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10a86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="10a86-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10a86-118">Request headers</span></span>

| <span data-ttu-id="10a86-119">Nome</span><span class="sxs-lookup"><span data-stu-id="10a86-119">Name</span></span>       | <span data-ttu-id="10a86-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a86-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="10a86-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="10a86-121">Authorization</span></span> | <span data-ttu-id="10a86-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="10a86-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10a86-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10a86-123">Request body</span></span>

<span data-ttu-id="10a86-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="10a86-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="10a86-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="10a86-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="10a86-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="10a86-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="10a86-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10a86-127">Property</span></span>     | <span data-ttu-id="10a86-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a86-128">Type</span></span>        | <span data-ttu-id="10a86-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a86-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10a86-130">description</span><span class="sxs-lookup"><span data-stu-id="10a86-130">description</span></span>|<span data-ttu-id="10a86-131">String</span><span class="sxs-lookup"><span data-stu-id="10a86-131">String</span></span>| <span data-ttu-id="10a86-132">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="10a86-132">The description for the role definition.</span></span> <span data-ttu-id="10a86-133">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="10a86-134">displayName</span><span class="sxs-lookup"><span data-stu-id="10a86-134">displayName</span></span>|<span data-ttu-id="10a86-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a86-135">String</span></span>| <span data-ttu-id="10a86-136">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="10a86-136">The display name for the role definition.</span></span> <span data-ttu-id="10a86-137">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="10a86-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a86-138">Required.</span></span>|
|<span data-ttu-id="10a86-139">id</span><span class="sxs-lookup"><span data-stu-id="10a86-139">id</span></span>|<span data-ttu-id="10a86-140">String</span><span class="sxs-lookup"><span data-stu-id="10a86-140">String</span></span>| <span data-ttu-id="10a86-141">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="10a86-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="10a86-142">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a86-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="10a86-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="10a86-143">isBuiltIn</span></span>|<span data-ttu-id="10a86-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="10a86-144">Boolean</span></span>| <span data-ttu-id="10a86-145">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="10a86-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="10a86-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10a86-146">Read-only.</span></span> |
|<span data-ttu-id="10a86-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="10a86-147">isEnabled</span></span>|<span data-ttu-id="10a86-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="10a86-148">Boolean</span></span>| <span data-ttu-id="10a86-149">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="10a86-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="10a86-150">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="10a86-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="10a86-151">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="10a86-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="10a86-152">resourceScopes</span></span>|<span data-ttu-id="10a86-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a86-153">String collection</span></span>| <span data-ttu-id="10a86-154">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="10a86-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="10a86-155">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="10a86-155">Currently only "/" is supported.</span></span> <span data-ttu-id="10a86-156">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-156">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="10a86-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="10a86-157">rolePermissions</span></span>|<span data-ttu-id="10a86-158">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="10a86-158">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="10a86-159">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="10a86-159">List of permissions included in the role.</span></span> <span data-ttu-id="10a86-160">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-160">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="10a86-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a86-161">Required.</span></span> |
|<span data-ttu-id="10a86-162">templateId</span><span class="sxs-lookup"><span data-stu-id="10a86-162">templateId</span></span>|<span data-ttu-id="10a86-163">String</span><span class="sxs-lookup"><span data-stu-id="10a86-163">String</span></span>| <span data-ttu-id="10a86-164">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="10a86-164">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="10a86-165">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="10a86-165">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="10a86-166">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-166">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="10a86-167">versão</span><span class="sxs-lookup"><span data-stu-id="10a86-167">version</span></span>|<span data-ttu-id="10a86-168">String</span><span class="sxs-lookup"><span data-stu-id="10a86-168">String</span></span>| <span data-ttu-id="10a86-169">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="10a86-169">Indicates version of the role definition.</span></span> <span data-ttu-id="10a86-170">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="10a86-170">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="10a86-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a86-171">Response</span></span>

<span data-ttu-id="10a86-172">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10a86-172">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10a86-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10a86-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="10a86-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a86-174">Request</span></span>

<span data-ttu-id="10a86-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="10a86-175">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10a86-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a86-176">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="10a86-177">C#</span><span class="sxs-lookup"><span data-stu-id="10a86-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10a86-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a86-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10a86-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10a86-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10a86-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a86-180">Response</span></span>

<span data-ttu-id="10a86-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="10a86-181">The following is an example of the response.</span></span>

> <span data-ttu-id="10a86-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10a86-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
