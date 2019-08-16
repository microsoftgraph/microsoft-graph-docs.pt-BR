---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd76b6baa201315dc21ae5b8f610f6c58233b37f
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437752"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="a6a76-103">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a6a76-103">Update unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6a76-104">Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="a6a76-104">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6a76-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6a76-105">Permissions</span></span>

<span data-ttu-id="a6a76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6a76-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6a76-108">Permission type</span></span>                        | <span data-ttu-id="a6a76-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6a76-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6a76-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6a76-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6a76-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a6a76-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="a6a76-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6a76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6a76-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6a76-113">Not supported.</span></span> |
| <span data-ttu-id="a6a76-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a76-114">Application</span></span>                            | <span data-ttu-id="a6a76-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="a6a76-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6a76-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6a76-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a6a76-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a76-117">Request headers</span></span>

| <span data-ttu-id="a6a76-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a6a76-118">Name</span></span>       | <span data-ttu-id="a6a76-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a76-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a6a76-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6a76-120">Authorization</span></span> | <span data-ttu-id="a6a76-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a6a76-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6a76-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a76-122">Request body</span></span>

<span data-ttu-id="a6a76-123">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a6a76-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a6a76-124">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a6a76-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a6a76-125">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a6a76-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6a76-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6a76-126">Property</span></span>     | <span data-ttu-id="a6a76-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6a76-127">Type</span></span>        | <span data-ttu-id="a6a76-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a76-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6a76-129">description</span><span class="sxs-lookup"><span data-stu-id="a6a76-129">description</span></span>|<span data-ttu-id="a6a76-130">String</span><span class="sxs-lookup"><span data-stu-id="a6a76-130">String</span></span>| <span data-ttu-id="a6a76-131">A descrição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a6a76-131">The description for the role definition.</span></span> <span data-ttu-id="a6a76-132">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="a6a76-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a76-133">displayName</span></span>|<span data-ttu-id="a6a76-134">String</span><span class="sxs-lookup"><span data-stu-id="a6a76-134">String</span></span>| <span data-ttu-id="a6a76-135">O nome de exibição da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a6a76-135">The display name for the role definition.</span></span> <span data-ttu-id="a6a76-136">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="a6a76-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6a76-137">Required.</span></span>|
|<span data-ttu-id="a6a76-138">id</span><span class="sxs-lookup"><span data-stu-id="a6a76-138">id</span></span>|<span data-ttu-id="a6a76-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a76-139">String</span></span>| <span data-ttu-id="a6a76-140">O identificador exclusivo da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a6a76-140">The unique identifier for the role definition.</span></span> <span data-ttu-id="a6a76-141">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6a76-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="a6a76-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a6a76-142">isBuiltIn</span></span>|<span data-ttu-id="a6a76-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6a76-143">Boolean</span></span>| <span data-ttu-id="a6a76-144">Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="a6a76-144">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="a6a76-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6a76-145">Read-only.</span></span> |
|<span data-ttu-id="a6a76-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="a6a76-146">isEnabled</span></span>|<span data-ttu-id="a6a76-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a76-147">Boolean</span></span>| <span data-ttu-id="a6a76-148">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a6a76-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="a6a76-149">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="a6a76-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="a6a76-150">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="a6a76-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a6a76-151">resourceScopes</span></span>|<span data-ttu-id="a6a76-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6a76-152">String collection</span></span>| <span data-ttu-id="a6a76-153">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="a6a76-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="a6a76-154">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="a6a76-154">Currently only "/" is supported.</span></span> <span data-ttu-id="a6a76-155">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-155">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="a6a76-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a6a76-156">rolePermissions</span></span>|<span data-ttu-id="a6a76-157">coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a6a76-157">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="a6a76-158">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="a6a76-158">List of permissions included in the role.</span></span> <span data-ttu-id="a6a76-159">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-159">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="a6a76-160">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6a76-160">Required.</span></span> |
|<span data-ttu-id="a6a76-161">templateId</span><span class="sxs-lookup"><span data-stu-id="a6a76-161">templateId</span></span>|<span data-ttu-id="a6a76-162">String</span><span class="sxs-lookup"><span data-stu-id="a6a76-162">String</span></span>| <span data-ttu-id="a6a76-163">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="a6a76-163">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="a6a76-164">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="a6a76-164">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="a6a76-165">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-165">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="a6a76-166">versão</span><span class="sxs-lookup"><span data-stu-id="a6a76-166">version</span></span>|<span data-ttu-id="a6a76-167">String</span><span class="sxs-lookup"><span data-stu-id="a6a76-167">String</span></span>| <span data-ttu-id="a6a76-168">Indica a versão da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a6a76-168">Indicates version of the role definition.</span></span> <span data-ttu-id="a6a76-169">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="a6a76-169">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="a6a76-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a76-170">Response</span></span>

<span data-ttu-id="a6a76-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a76-171">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a76-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6a76-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6a76-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a76-173">Request</span></span>

<span data-ttu-id="a6a76-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6a76-174">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6a76-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a76-175">Response</span></span>

<span data-ttu-id="a6a76-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a76-176">The following is an example of the response.</span></span>

> <span data-ttu-id="a6a76-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6a76-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
