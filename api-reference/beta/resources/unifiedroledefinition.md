---
title: tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9f9b45885219a081bad8d7f34a49f81d8062d212
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519607"
---
# <a name="unifiedroledefinition-resource-type"></a>tipo de recurso unifiedRoleDefinition

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleDefinition é uma coleção de permissões que lista as operações que podem ser executadas, como leitura, gravação e exclusão.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | coleção [unifiedRoleDefinition](unifiedroledefinition.md) | Leia uma lista de objetos unifiedRoleDefinition e suas propriedades. |
| [Obter unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Ler as propriedades de um objeto unifiedRoleDefinition. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Criar um objeto unifiedRoleDefinition. |
| [Atualizar unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Atualizar um objeto unifiedRoleDefinition. |
| [Excluir unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Nenhum | Excluir um objeto unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String| A descrição para o unifiedRoleDefinition. Somente leitura quando isbuiltem for true. |
|displayName|Cadeia de caracteres| O nome de exibição do unifiedRoleDefinition. Somente leitura quando isbuiltem for true. Obrigatório.|
|id|String| O identificador exclusivo para o unifiedRoleDefinition. Chave, não anulável, somente leitura. |
|isBuiltIn|Booliano| Sinalizador que indica se o unifiedRoleDefinition é parte do conjunto padrão incluído no produto ou personalizado. Somente leitura. |
|isEnabled|Boolean| Sinalizador que indica se a função está habilitada para atribuição. Se false, a função não estará disponível para atribuição. Somente leitura quando isbuiltem for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de escopos permissões concedidas pela definição de função aplicam-se ao. No momento, só há suporte para "/". Somente leitura quando isbuiltem for true. |
|rolePermissions|coleção [unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando isbuiltem for true. Obrigatório. |
|templateId|String| Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso. Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios. Somente leitura quando isbuiltem for true. |
|versão|String| Indica a versão do unifiedRoleDefinition. Somente leitura quando isbuiltem for true.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
