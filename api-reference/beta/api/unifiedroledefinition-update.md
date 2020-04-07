---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e9ff2d3f61e1ce6e2809ae38fccbc4029ab49852
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160258"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="ae2e6-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ae2e6-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="ae2e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae2e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae2e6-105">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="ae2e6-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae2e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae2e6-106">Permissions</span></span>

<span data-ttu-id="ae2e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae2e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae2e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae2e6-109">Permission type</span></span>                        | <span data-ttu-id="ae2e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae2e6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae2e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae2e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae2e6-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="ae2e6-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="ae2e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae2e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae2e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-114">Not supported.</span></span> |
| <span data-ttu-id="ae2e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae2e6-115">Application</span></span>                            | <span data-ttu-id="ae2e6-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="ae2e6-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae2e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae2e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ae2e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2e6-118">Request headers</span></span>

| <span data-ttu-id="ae2e6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ae2e6-119">Name</span></span>       | <span data-ttu-id="ae2e6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae2e6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ae2e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae2e6-121">Authorization</span></span> | <span data-ttu-id="ae2e6-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ae2e6-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae2e6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2e6-123">Request body</span></span>

<span data-ttu-id="ae2e6-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ae2e6-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ae2e6-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ae2e6-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae2e6-127">Property</span></span>     | <span data-ttu-id="ae2e6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae2e6-128">Type</span></span>        | <span data-ttu-id="ae2e6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae2e6-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae2e6-130">description</span><span class="sxs-lookup"><span data-stu-id="ae2e6-130">description</span></span>|<span data-ttu-id="ae2e6-131">String</span><span class="sxs-lookup"><span data-stu-id="ae2e6-131">String</span></span>| <span data-ttu-id="ae2e6-132">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-132">The description for the role definition.</span></span> <span data-ttu-id="ae2e6-133">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-133">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ae2e6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2e6-134">displayName</span></span>|<span data-ttu-id="ae2e6-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae2e6-135">String</span></span>| <span data-ttu-id="ae2e6-136">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-136">The display name for the role definition.</span></span> <span data-ttu-id="ae2e6-137">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-137">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ae2e6-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-138">Required.</span></span>|
|<span data-ttu-id="ae2e6-139">id</span><span class="sxs-lookup"><span data-stu-id="ae2e6-139">id</span></span>|<span data-ttu-id="ae2e6-140">String</span><span class="sxs-lookup"><span data-stu-id="ae2e6-140">String</span></span>| <span data-ttu-id="ae2e6-141">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-141">The unique identifier for the role definition.</span></span> <span data-ttu-id="ae2e6-142">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-142">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="ae2e6-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ae2e6-143">isBuiltIn</span></span>|<span data-ttu-id="ae2e6-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae2e6-144">Boolean</span></span>| <span data-ttu-id="ae2e6-145">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-145">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="ae2e6-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-146">Read-only.</span></span> |
|<span data-ttu-id="ae2e6-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ae2e6-147">isEnabled</span></span>|<span data-ttu-id="ae2e6-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae2e6-148">Boolean</span></span>| <span data-ttu-id="ae2e6-149">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-149">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="ae2e6-150">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-150">If false the role is not available for assignment.</span></span> <span data-ttu-id="ae2e6-151">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-151">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ae2e6-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ae2e6-152">resourceScopes</span></span>|<span data-ttu-id="ae2e6-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae2e6-153">String collection</span></span>| <span data-ttu-id="ae2e6-154">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-154">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="ae2e6-155">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="ae2e6-155">Currently only "/" is supported.</span></span> <span data-ttu-id="ae2e6-156">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-156">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ae2e6-157">**NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**</span><span class="sxs-lookup"><span data-stu-id="ae2e6-157">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="ae2e6-158">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ae2e6-158">rolePermissions</span></span>|<span data-ttu-id="ae2e6-159">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ae2e6-159">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="ae2e6-160">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-160">List of permissions included in the role.</span></span> <span data-ttu-id="ae2e6-161">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-161">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="ae2e6-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-162">Required.</span></span> |
|<span data-ttu-id="ae2e6-163">templateId</span><span class="sxs-lookup"><span data-stu-id="ae2e6-163">templateId</span></span>|<span data-ttu-id="ae2e6-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae2e6-164">String</span></span>| <span data-ttu-id="ae2e6-165">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-165">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="ae2e6-166">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-166">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="ae2e6-167">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="ae2e6-168">versão</span><span class="sxs-lookup"><span data-stu-id="ae2e6-168">version</span></span>|<span data-ttu-id="ae2e6-169">String</span><span class="sxs-lookup"><span data-stu-id="ae2e6-169">String</span></span>| <span data-ttu-id="ae2e6-170">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-170">Indicates version of the role definition.</span></span> <span data-ttu-id="ae2e6-171">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-171">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="ae2e6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae2e6-172">Response</span></span>

<span data-ttu-id="ae2e6-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-173">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae2e6-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae2e6-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae2e6-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae2e6-175">Request</span></span>

<span data-ttu-id="ae2e6-176">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-176">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="ae2e6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae2e6-177">Response</span></span>

<span data-ttu-id="ae2e6-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-178">The following is an example of the response.</span></span>
> <span data-ttu-id="ae2e6-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae2e6-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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