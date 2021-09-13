---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função é uma coleção de permissões Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2307b6fd429e8cc4942a5a50e04316ee77332671
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148494"
---
# <a name="unifiedroledefinition-resource-type"></a>Tipo de recurso unifiedRoleDefinition

Namespace: microsoft.graph

Uma definição de função é uma coleção de permissões no Azure Active Directory (Azure AD) listando as operações que podem ser executadas e os recursos nos quais eles podem ser executados.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Leia uma lista de objetos unifiedRoleDefinition e suas propriedades. |
| [Obter unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Leia as propriedades de um objeto unifiedRoleDefinition. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um objeto unifiedRoleDefinition. |
| [Atualizar unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Atualize um objeto unifiedRoleDefinition. |
| [Excluir unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Nenhum(a) | Exclua um objeto unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres| A descrição do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** é `true` . |
|displayName|String| O nome de exibição do unifiedRoleDefinition. Somente leitura quando **isBuiltIn** é `true` . Obrigatório.  Suporta $filter ( `eq` , `in` ).|
|id|String| O identificador exclusivo para a definição de função. Chave, não anulada, somente leitura. Herdado da [entidade](../resources/entity.md). Suporta $filter ( `eq` , `in` ). |
|isBuiltIn|Booliano| Sinalizador indicando se a definição de função faz parte do conjunto padrão incluído no Azure Active Directory (Azure AD) ou uma definição personalizada. Somente leitura. Suporta $filter ( `eq` , `in` ). |
|isEnabled|Booliano| Sinalizador indicando se a função está habilitada para atribuição. Se `false` a função não estiver disponível para atribuição. Somente leitura quando **isBuiltIn** for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista dos escopos ou permissões aos que a definição de função se aplica. Atualmente, `/` só há suporte. Somente leitura quando **isBuiltIn** for true. **NÃO USE. Isso será preterido em breve. Anexar escopo à atribuição de função.** | 
|rolePermissions|[Coleção unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando **isBuiltIn** é `true` . Obrigatório. |
|templateId|String| Identificador de modelo personalizado que pode ser definido quando **isBuiltIn** é, mas é somente leitura `false` quando **isBuiltIn** é `true` . Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes. |
|versão|String| Indica a versão da definição de função. Somente leitura quando **isBuiltIn** é `true` .|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [Coleção unifiedRoleDefinition](unifiedroledefinition.md)| Coleção somente leitura de definições de função que a definição de função determinada herda. Somente funções do Azure AD integrados (**isBuiltIn** `true` é ) suportam esse atributo. Suporta o `$expand`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleDefinition",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isBuiltIn": "Boolean",
  "isEnabled": "Boolean",
  "resourceScopes": [
    "String"
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.unifiedRolePermission"
    }
  ],
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

