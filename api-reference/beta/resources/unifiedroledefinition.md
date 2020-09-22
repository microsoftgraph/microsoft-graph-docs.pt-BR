---
title: tipo de recurso unifiedRoleDefinition
description: Uma definição de função unificada é uma coleção de permissões
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2ff58263a6fb28d41c79eaca721a791dab37992
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988750"
---
# <a name="unifiedroledefinition-resource-type"></a>tipo de recurso unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleDefinition é uma coleção de permissões que lista as operações que podem ser executadas, como leitura, gravação e exclusão.

## <a name="methods"></a>Methods

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
|displayName|String| O nome de exibição do unifiedRoleDefinition. Somente leitura quando isbuiltem for true. Obrigatório.|
|id|String| O identificador exclusivo para o unifiedRoleDefinition. Chave, não anulável, somente leitura. |
|isBuiltIn|Booliano| Sinalizador que indica se o unifiedRoleDefinition é parte do conjunto padrão incluído no produto ou personalizado. Somente leitura. |
|isEnabled|Boolean| Sinalizador que indica se a função está habilitada para atribuição. Se false, a função não estará disponível para atribuição. Somente leitura quando isbuiltem for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de escopos permissões concedidas pela definição de função aplicam-se ao. No momento, só há suporte para "/". Somente leitura quando isbuiltem for true. **NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função** | 
|rolePermissions|coleção [unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando isbuiltem for true. Obrigatório. |
|templateId|String| Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso. Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios. Somente leitura quando isbuiltem for true. |
|inheritsPermissionsFrom| coleção [unifiedRoleDefinition](unifiedroledefinition.md)| Coleção somente leitura de definições de função que a definição de função fornecida herda. Somente as funções internas do Azure AD dão suporte a esse atributo. |
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


