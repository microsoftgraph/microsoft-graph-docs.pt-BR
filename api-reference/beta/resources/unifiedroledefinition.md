---
title: tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: be1b8a0b1a623c6cf322d5cf7997f04b87875c51
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437745"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="e6248-103">tipo de recurso unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-103">unifiedRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6248-104">Um unifiedRoleDefinition é uma coleção de permissões que lista as operações que podem ser executadas, como leitura, gravação e exclusão.</span><span class="sxs-lookup"><span data-stu-id="e6248-104">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="e6248-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6248-105">Methods</span></span>

| <span data-ttu-id="e6248-106">Método</span><span class="sxs-lookup"><span data-stu-id="e6248-106">Method</span></span>       | <span data-ttu-id="e6248-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6248-107">Return Type</span></span> | <span data-ttu-id="e6248-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6248-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e6248-109">Listar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-109">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="e6248-110">coleção [unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e6248-110">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="e6248-111">Leia uma lista de objetos unifiedRoleDefinition e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e6248-111">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="e6248-112">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-112">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="e6248-113">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-113">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="e6248-114">Ler as propriedades de um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-114">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="e6248-115">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-115">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="e6248-116">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-116">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="e6248-117">Criar um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-117">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="e6248-118">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-118">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="e6248-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="e6248-120">Atualizar um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-120">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="e6248-121">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6248-121">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="e6248-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6248-122">None</span></span> | <span data-ttu-id="e6248-123">Excluir um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-123">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6248-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6248-124">Properties</span></span>

| <span data-ttu-id="e6248-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6248-125">Property</span></span>     | <span data-ttu-id="e6248-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6248-126">Type</span></span>        | <span data-ttu-id="e6248-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6248-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6248-128">description</span><span class="sxs-lookup"><span data-stu-id="e6248-128">description</span></span>|<span data-ttu-id="e6248-129">String</span><span class="sxs-lookup"><span data-stu-id="e6248-129">String</span></span>| <span data-ttu-id="e6248-130">A descrição para o unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-130">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="e6248-131">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-131">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e6248-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e6248-132">displayName</span></span>|<span data-ttu-id="e6248-133">String</span><span class="sxs-lookup"><span data-stu-id="e6248-133">String</span></span>| <span data-ttu-id="e6248-134">O nome de exibição do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-134">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="e6248-135">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-135">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e6248-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6248-136">Required.</span></span>|
|<span data-ttu-id="e6248-137">id</span><span class="sxs-lookup"><span data-stu-id="e6248-137">id</span></span>|<span data-ttu-id="e6248-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6248-138">String</span></span>| <span data-ttu-id="e6248-139">O identificador exclusivo para o unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-139">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="e6248-140">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6248-140">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="e6248-141">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e6248-141">isBuiltIn</span></span>|<span data-ttu-id="e6248-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6248-142">Boolean</span></span>| <span data-ttu-id="e6248-143">Sinalizador que indica se o unifiedRoleDefinition é parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="e6248-143">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="e6248-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6248-144">Read-only.</span></span> |
|<span data-ttu-id="e6248-145">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e6248-145">isEnabled</span></span>|<span data-ttu-id="e6248-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6248-146">Boolean</span></span>| <span data-ttu-id="e6248-147">Sinalizador que indica se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="e6248-147">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="e6248-148">Se false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="e6248-148">If false the role is not available for assignment.</span></span> <span data-ttu-id="e6248-149">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-149">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e6248-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e6248-150">resourceScopes</span></span>|<span data-ttu-id="e6248-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6248-151">String collection</span></span>| <span data-ttu-id="e6248-152">Lista de escopos permissões concedidas pela definição de função aplicam-se ao.</span><span class="sxs-lookup"><span data-stu-id="e6248-152">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="e6248-153">No momento, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="e6248-153">Currently only "/" is supported.</span></span> <span data-ttu-id="e6248-154">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-154">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e6248-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e6248-155">rolePermissions</span></span>|<span data-ttu-id="e6248-156">coleção [unifiedRolePermission](unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="e6248-156">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="e6248-157">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="e6248-157">List of permissions included in the role.</span></span> <span data-ttu-id="e6248-158">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-158">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="e6248-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6248-159">Required.</span></span> |
|<span data-ttu-id="e6248-160">templateId</span><span class="sxs-lookup"><span data-stu-id="e6248-160">templateId</span></span>|<span data-ttu-id="e6248-161">String</span><span class="sxs-lookup"><span data-stu-id="e6248-161">String</span></span>| <span data-ttu-id="e6248-162">Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso.</span><span class="sxs-lookup"><span data-stu-id="e6248-162">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="e6248-163">Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios.</span><span class="sxs-lookup"><span data-stu-id="e6248-163">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="e6248-164">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-164">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="e6248-165">versão</span><span class="sxs-lookup"><span data-stu-id="e6248-165">version</span></span>|<span data-ttu-id="e6248-166">String</span><span class="sxs-lookup"><span data-stu-id="e6248-166">String</span></span>| <span data-ttu-id="e6248-167">Indica a versão do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e6248-167">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="e6248-168">Somente leitura quando isbuiltem for true.</span><span class="sxs-lookup"><span data-stu-id="e6248-168">Read-only when isBuiltIn is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6248-169">Relações</span><span class="sxs-lookup"><span data-stu-id="e6248-169">Relationships</span></span>

<span data-ttu-id="e6248-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6248-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6248-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6248-171">JSON representation</span></span>

<span data-ttu-id="e6248-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6248-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": true,
  "isEnabled": true,
  "resourceScopes": ["String"],
  "rolePermissions": [{"@odata.type": "microsoft.graph.unifiedRolePermission"}],
  "templateId": "String",
  "version": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
