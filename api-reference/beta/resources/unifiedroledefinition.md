---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é um conjunto de permissões
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d146f215586533b9564d267c686a437f1314d54b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159826"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="8ec15-103">Tipo de recurso unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="8ec15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ec15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec15-105">Um unifiedRoleDefinition é uma coleção de permissões listando as operações que podem ser executadas, como ler, gravar e excluir.</span><span class="sxs-lookup"><span data-stu-id="8ec15-105">A unifiedRoleDefinition is a collection of permissions listing the operations that can be performed, such as read, write, and delete.</span></span>

## <a name="methods"></a><span data-ttu-id="8ec15-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ec15-106">Methods</span></span>

| <span data-ttu-id="8ec15-107">Método</span><span class="sxs-lookup"><span data-stu-id="8ec15-107">Method</span></span>       | <span data-ttu-id="8ec15-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ec15-108">Return Type</span></span> | <span data-ttu-id="8ec15-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec15-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8ec15-110">Listar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-110">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="8ec15-111">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8ec15-111">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="8ec15-112">Leia uma lista de objetos unifiedRoleDefinition e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8ec15-112">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="8ec15-113">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-113">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="8ec15-114">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-114">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="8ec15-115">Leia as propriedades de um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-115">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="8ec15-116">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-116">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="8ec15-117">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-117">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="8ec15-118">Crie um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-118">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="8ec15-119">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-119">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="8ec15-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="8ec15-121">Atualize um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-121">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="8ec15-122">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8ec15-122">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="8ec15-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8ec15-123">None</span></span> | <span data-ttu-id="8ec15-124">Exclua um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-124">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ec15-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ec15-125">Properties</span></span>

| <span data-ttu-id="8ec15-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ec15-126">Property</span></span>     | <span data-ttu-id="8ec15-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ec15-127">Type</span></span>        | <span data-ttu-id="8ec15-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec15-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ec15-129">description</span><span class="sxs-lookup"><span data-stu-id="8ec15-129">description</span></span>|<span data-ttu-id="8ec15-130">String</span><span class="sxs-lookup"><span data-stu-id="8ec15-130">String</span></span>| <span data-ttu-id="8ec15-131">A descrição da unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-131">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="8ec15-132">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-132">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="8ec15-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8ec15-133">displayName</span></span>|<span data-ttu-id="8ec15-134">String</span><span class="sxs-lookup"><span data-stu-id="8ec15-134">String</span></span>| <span data-ttu-id="8ec15-135">O nome de exibição para unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-135">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="8ec15-136">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-136">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="8ec15-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ec15-137">Required.</span></span>|
|<span data-ttu-id="8ec15-138">id</span><span class="sxs-lookup"><span data-stu-id="8ec15-138">id</span></span>|<span data-ttu-id="8ec15-139">String</span><span class="sxs-lookup"><span data-stu-id="8ec15-139">String</span></span>| <span data-ttu-id="8ec15-140">O identificador exclusivo da unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-140">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="8ec15-141">Chave, não anulada, Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ec15-141">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="8ec15-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8ec15-142">isBuiltIn</span></span>|<span data-ttu-id="8ec15-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8ec15-143">Boolean</span></span>| <span data-ttu-id="8ec15-144">Sinalizador indicando se unifiedRoleDefinition faz parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="8ec15-144">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="8ec15-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ec15-145">Read-only.</span></span> |
|<span data-ttu-id="8ec15-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8ec15-146">isEnabled</span></span>|<span data-ttu-id="8ec15-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="8ec15-147">Boolean</span></span>| <span data-ttu-id="8ec15-148">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="8ec15-148">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="8ec15-149">Se for falso, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="8ec15-149">If false the role is not available for assignment.</span></span> <span data-ttu-id="8ec15-150">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-150">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="8ec15-151">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="8ec15-151">resourceScopes</span></span>|<span data-ttu-id="8ec15-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ec15-152">String collection</span></span>| <span data-ttu-id="8ec15-153">A lista de permissões de escopos concedidas pela definição de função se aplica.</span><span class="sxs-lookup"><span data-stu-id="8ec15-153">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="8ec15-154">Atualmente, só há suporte para "/".</span><span class="sxs-lookup"><span data-stu-id="8ec15-154">Currently only "/" is supported.</span></span> <span data-ttu-id="8ec15-155">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-155">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="8ec15-156">**NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função**</span><span class="sxs-lookup"><span data-stu-id="8ec15-156">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="8ec15-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8ec15-157">rolePermissions</span></span>|<span data-ttu-id="8ec15-158">[Coleção unifiedRolePermission](unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="8ec15-158">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="8ec15-159">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="8ec15-159">List of permissions included in the role.</span></span> <span data-ttu-id="8ec15-160">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-160">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="8ec15-161">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ec15-161">Required.</span></span> |
|<span data-ttu-id="8ec15-162">templateId</span><span class="sxs-lookup"><span data-stu-id="8ec15-162">templateId</span></span>|<span data-ttu-id="8ec15-163">String</span><span class="sxs-lookup"><span data-stu-id="8ec15-163">String</span></span>| <span data-ttu-id="8ec15-164">Identificador de modelo personalizado que pode ser definido quando isBuiltIn é falso.</span><span class="sxs-lookup"><span data-stu-id="8ec15-164">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="8ec15-165">Esse identificador é geralmente usado se um identificador precisa ser o mesmo em diretórios diferentes.</span><span class="sxs-lookup"><span data-stu-id="8ec15-165">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="8ec15-166">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-166">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="8ec15-167">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="8ec15-167">inheritsPermissionsFrom</span></span>| <span data-ttu-id="8ec15-168">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8ec15-168">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="8ec15-169">Coleção somente leitura de definições de função que a definição de função determinada herda.</span><span class="sxs-lookup"><span data-stu-id="8ec15-169">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="8ec15-170">Somente funções do Azure AD integrados suportam esse atributo.</span><span class="sxs-lookup"><span data-stu-id="8ec15-170">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="8ec15-171">versão</span><span class="sxs-lookup"><span data-stu-id="8ec15-171">version</span></span>|<span data-ttu-id="8ec15-172">String</span><span class="sxs-lookup"><span data-stu-id="8ec15-172">String</span></span>| <span data-ttu-id="8ec15-173">Indica a versão do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="8ec15-173">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="8ec15-174">Somente leitura quando isBuiltIn for verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="8ec15-174">Read-only when isBuiltIn is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ec15-175">Relações</span><span class="sxs-lookup"><span data-stu-id="8ec15-175">Relationships</span></span>

<span data-ttu-id="8ec15-176">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ec15-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ec15-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ec15-177">JSON representation</span></span>

<span data-ttu-id="8ec15-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ec15-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
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
  "inheritsPermissionsFrom": [{"@odata.type": "microsoft.graph.unifiedRoleDefinition"}],
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


