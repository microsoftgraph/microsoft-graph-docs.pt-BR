---
title: Tipo de recurso unifiedRoleDefinition
description: Uma definição de função é uma coleção de permissões Azure Active Directory (Azure AD).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f3a54d12ce4c11ee10d106759ccbaa0e32b80978
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246591"
---
# <a name="unifiedroledefinition-resource-type"></a>Tipo de recurso unifiedRoleDefinition

Namespace: microsoft.graph

Uma definição de função é uma coleção de permissões em Azure Active Directory (Azure AD) listando as operações que podem ser executadas e os recursos nos quais elas podem ser executadas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleDefinition](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Leia uma lista de objetos unifiedRoleDefinition e suas propriedades. |
| [Obter unifiedRoleDefinition](../api/unifiedroledefinition-get.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Leia as propriedades de um objeto unifiedRoleDefinition. |
| [Criar roleDefinitions](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um objeto unifiedRoleDefinition. |
| [Atualizar unifiedRoleDefinition](../api/unifiedroledefinition-update.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Atualize um objeto unifiedRoleDefinition. |
| [Excluir unifiedRoleDefinition](../api/unifiedroledefinition-delete.md) | Nenhum | Exclua um objeto unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres| A descrição para unifiedRoleDefinition. Somente leitura quando **isBuiltIn** é `true`. |
|displayName|Cadeia de caracteres| O nome de exibição para unifiedRoleDefinition. Somente leitura quando **isBuiltIn** é `true`. Obrigatório.  Dá $filter (`eq`, `in`).|
|id|Cadeia de caracteres| O identificador exclusivo para a definição de função. Chave, não anulável, somente leitura. Herdado da [entidade](../resources/entity.md). Dá $filter (`eq`, `in`). |
|isBuiltIn|Booliano| Sinalizador que indica se a definição de função faz parte do conjunto padrão incluído Azure Active Directory (Azure AD) ou uma definição personalizada. Somente leitura. Dá $filter (`eq`, `in`). |
|isEnabled|Booliano| Sinalizador que indica se a função está habilitada para atribuição. Se `false` a função não estiver disponível para atribuição. Somente leitura quando **isBuiltIn** for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de escopos ou permissões aos quais a definição de função se aplica. Atualmente, há suporte `/` apenas. Somente leitura quando **isBuiltIn** for true. **NÃO USE. Isso será preterido em breve. Anexe o escopo à atribuição de função.** | 
|rolePermissions|[Coleção unifiedRolePermission](unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando **isBuiltIn** é `true`. Obrigatório. |
|Templateid|Cadeia de caracteres| Identificador de modelo personalizado que pode ser definido quando **isBuiltIn** é `false` , mas é somente leitura quando **isBuiltIn** é `true`. Esse identificador normalmente é usado se for necessário que um identificador seja o mesmo em diretórios diferentes. |
|versão|String| Indica a versão da definição de função. Somente leitura quando **isBuiltIn** é `true`.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|inheritsPermissionsFrom| [Coleção unifiedRoleDefinition](unifiedroledefinition.md)| Coleção somente leitura de definições de função da qual a definição de função fornecida herda. Somente Azure AD funções internas (**isBuiltIn** é`true`) dão suporte a esse atributo. Suporta o `$expand`. |

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

