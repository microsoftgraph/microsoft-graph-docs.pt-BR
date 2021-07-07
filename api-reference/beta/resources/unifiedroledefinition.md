---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 804315ae2ae4b803088a419913ca91c11a8e51c4
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316491"
---
# <a name="unifiedroledefinition-resource-type"></a><span data-ttu-id="89930-103">Tipo de recurso unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-103">unifiedRoleDefinition resource type</span></span>

<span data-ttu-id="89930-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89930-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89930-105">Representa uma coleção de permissões que listam as operações, como leitura, gravação e exclusão, que podem ser executadas [](rolemanagement.md)por um provedor RBAC, como parte do gerenciamento de função RBAC Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="89930-105">Represents a collection of permissions listing the operations, such as read, write, and delete, that can be performed by an RBAC provider, as part of Microsoft 365 RBAC [role management](rolemanagement.md).</span></span>

<span data-ttu-id="89930-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="89930-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="89930-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="89930-107">cloud PC</span></span> 
- <span data-ttu-id="89930-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="89930-108">device management (Intune)</span></span>
- <span data-ttu-id="89930-109">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="89930-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="89930-110">gerenciamento de direitos (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="89930-110">entitlement management (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="89930-111">No momento, os provedores de RBAC de gerenciamento de direitos e pc na nuvem suportam apenas a [lista](../api/rbacapplication-list-roledefinitions.md) e [obter](../api/unifiedroledefinition-get.md) operações.</span><span class="sxs-lookup"><span data-stu-id="89930-111">The cloud PC and entitlement management RBAC providers currently support only the [list](../api/rbacapplication-list-roledefinitions.md) and [get](../api/unifiedroledefinition-get.md) operations.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="89930-112">Methods</span><span class="sxs-lookup"><span data-stu-id="89930-112">Methods</span></span>

| <span data-ttu-id="89930-113">Método</span><span class="sxs-lookup"><span data-stu-id="89930-113">Method</span></span>       | <span data-ttu-id="89930-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89930-114">Return Type</span></span> | <span data-ttu-id="89930-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="89930-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="89930-116">Listar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-116">List unifiedRoleDefinition</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="89930-117">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="89930-117">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="89930-118">Leia uma lista de objetos unifiedRoleDefinition e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="89930-118">Read a list of unifiedRoleDefinition objects, and their properties.</span></span> |
| [<span data-ttu-id="89930-119">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-119">Get unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-get.md) | [<span data-ttu-id="89930-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="89930-121">Leia as propriedades de um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-121">Read the properties of a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="89930-122">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-122">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="89930-123">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-123">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="89930-124">Crie um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-124">Create a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="89930-125">Atualizar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-125">Update unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-update.md) | [<span data-ttu-id="89930-126">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-126">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="89930-127">Atualize um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-127">Update a unifiedRoleDefinition object.</span></span> |
| [<span data-ttu-id="89930-128">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="89930-128">Delete unifiedRoleDefinition</span></span>](../api/unifiedroledefinition-delete.md) | <span data-ttu-id="89930-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89930-129">None</span></span> | <span data-ttu-id="89930-130">Exclua um objeto unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-130">Delete a unifiedRoleDefinition object.</span></span> |

## <a name="properties"></a><span data-ttu-id="89930-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89930-131">Properties</span></span>

| <span data-ttu-id="89930-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89930-132">Property</span></span>     | <span data-ttu-id="89930-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="89930-133">Type</span></span>        | <span data-ttu-id="89930-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="89930-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89930-135">description</span><span class="sxs-lookup"><span data-stu-id="89930-135">description</span></span>|<span data-ttu-id="89930-136">String</span><span class="sxs-lookup"><span data-stu-id="89930-136">String</span></span>| <span data-ttu-id="89930-137">A descrição do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-137">The description for the unifiedRoleDefinition.</span></span> <span data-ttu-id="89930-138">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-138">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="89930-139">displayName</span><span class="sxs-lookup"><span data-stu-id="89930-139">displayName</span></span>|<span data-ttu-id="89930-140">String</span><span class="sxs-lookup"><span data-stu-id="89930-140">String</span></span>| <span data-ttu-id="89930-141">O nome de exibição do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-141">The display name for the unifiedRoleDefinition.</span></span> <span data-ttu-id="89930-142">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-142">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="89930-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89930-143">Required.</span></span>  <span data-ttu-id="89930-144">Oferece `$filter` suporte ( e somente `eq` `startsWith` operadores).</span><span class="sxs-lookup"><span data-stu-id="89930-144">Supports `$filter` (`eq` and `startsWith` operators only).</span></span>|
|<span data-ttu-id="89930-145">id</span><span class="sxs-lookup"><span data-stu-id="89930-145">id</span></span>|<span data-ttu-id="89930-146">String</span><span class="sxs-lookup"><span data-stu-id="89930-146">String</span></span>| <span data-ttu-id="89930-147">O identificador exclusivo do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-147">The unique identifier for the unifiedRoleDefinition.</span></span> <span data-ttu-id="89930-148">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89930-148">Key, not nullable, Read-only.</span></span>  <span data-ttu-id="89930-149">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="89930-149">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="89930-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="89930-150">isBuiltIn</span></span>|<span data-ttu-id="89930-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="89930-151">Boolean</span></span>| <span data-ttu-id="89930-152">Sinalizador indicando se unifiedRoleDefinition faz parte do conjunto padrão incluído no produto ou personalizado.</span><span class="sxs-lookup"><span data-stu-id="89930-152">Flag indicating if the unifiedRoleDefinition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="89930-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89930-153">Read-only.</span></span>  <span data-ttu-id="89930-154">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="89930-154">Supports `$filter` (`eq` operator only).</span></span>|
|<span data-ttu-id="89930-155">isEnabled</span><span class="sxs-lookup"><span data-stu-id="89930-155">isEnabled</span></span>|<span data-ttu-id="89930-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="89930-156">Boolean</span></span>| <span data-ttu-id="89930-157">Sinalizador indicando se a função está habilitada para atribuição.</span><span class="sxs-lookup"><span data-stu-id="89930-157">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="89930-158">Se for false, a função não estará disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="89930-158">If false the role is not available for assignment.</span></span> <span data-ttu-id="89930-159">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-159">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="89930-160">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="89930-160">resourceScopes</span></span>|<span data-ttu-id="89930-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89930-161">String collection</span></span>| <span data-ttu-id="89930-162">Lista de permissões de escopo concedidas pela definição de função a que se aplicam.</span><span class="sxs-lookup"><span data-stu-id="89930-162">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="89930-163">Atualmente, `/` só há suporte.</span><span class="sxs-lookup"><span data-stu-id="89930-163">Currently only `/` is supported.</span></span> <span data-ttu-id="89930-164">Somente leitura quando isBuiltIn for true.</span><span class="sxs-lookup"><span data-stu-id="89930-164">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="89930-165">**NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função**</span><span class="sxs-lookup"><span data-stu-id="89930-165">**DO NOT USE. This is going to be deprecated soon. Attach scope to role assignment**</span></span> | 
|<span data-ttu-id="89930-166">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="89930-166">rolePermissions</span></span>|<span data-ttu-id="89930-167">[Coleção unifiedRolePermission](unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="89930-167">[unifiedRolePermission](unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="89930-168">Lista de permissões incluídas na função.</span><span class="sxs-lookup"><span data-stu-id="89930-168">List of permissions included in the role.</span></span> <span data-ttu-id="89930-169">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-169">Read-only when **isBuiltIn** is true.</span></span> <span data-ttu-id="89930-170">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89930-170">Required.</span></span> |
|<span data-ttu-id="89930-171">templateId</span><span class="sxs-lookup"><span data-stu-id="89930-171">templateId</span></span>|<span data-ttu-id="89930-172">String</span><span class="sxs-lookup"><span data-stu-id="89930-172">String</span></span>| <span data-ttu-id="89930-173">Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false.</span><span class="sxs-lookup"><span data-stu-id="89930-173">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="89930-174">Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes.</span><span class="sxs-lookup"><span data-stu-id="89930-174">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="89930-175">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-175">Read-only when **isBuiltIn** is true.</span></span> |
|<span data-ttu-id="89930-176">versão</span><span class="sxs-lookup"><span data-stu-id="89930-176">version</span></span>|<span data-ttu-id="89930-177">String</span><span class="sxs-lookup"><span data-stu-id="89930-177">String</span></span>| <span data-ttu-id="89930-178">Indica a versão do unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="89930-178">Indicates version of the unifiedRoleDefinition.</span></span> <span data-ttu-id="89930-179">Somente leitura quando **isBuiltIn** for true.</span><span class="sxs-lookup"><span data-stu-id="89930-179">Read-only when **isBuiltIn** is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89930-180">Relações</span><span class="sxs-lookup"><span data-stu-id="89930-180">Relationships</span></span>

| <span data-ttu-id="89930-181">Relação</span><span class="sxs-lookup"><span data-stu-id="89930-181">Relationship</span></span> | <span data-ttu-id="89930-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="89930-182">Type</span></span>   |<span data-ttu-id="89930-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="89930-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89930-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="89930-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="89930-185">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="89930-185">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="89930-186">Coleção somente leitura de definições de função que a definição de função determinada herda.</span><span class="sxs-lookup"><span data-stu-id="89930-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="89930-187">Somente funções do Azure AD integrados suportam esse atributo.</span><span class="sxs-lookup"><span data-stu-id="89930-187">Only Azure AD built-in roles support this attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89930-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89930-188">JSON representation</span></span>

<span data-ttu-id="89930-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89930-189">The following is a JSON representation of the resource.</span></span>

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


