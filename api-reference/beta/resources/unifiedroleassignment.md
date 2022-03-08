---
title: Tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o link entre uma definição de função e uma entidade principal em um escopo específico para a finalidade de conceder acesso.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b7500c3d332b26a3078ed16f3e589e5125deb9f8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335973"
---
# <a name="unifiedroleassignment-resource-type"></a>Tipo de recurso unifiedRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignment é usado para conceder acesso aos recursos. Ele representa uma definição de função atribuída a uma entidade principal (normalmente um usuário) em um escopo específico.

É necessário fornecer um directoryScopeId ou um appScopeId.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar unifiedRoleAssignment](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Leia uma lista de objetos unifiedRoleAssignment e suas propriedades. |
| [Listar transitiveRoleAssignments](../api/rbacapplication-list-transitiveroleassignments.md) | [Coleção unifiedRoleAssignment](unifiedroleassignment.md) | Obter unifiedRoleAssignments diretos e transitivos atribuídos a uma entidade de segurança específica. A especificação de principalId é necessária. |
| [Obter unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Leia propriedades e relações do objeto unifiedRoleAssignment. |
| [Criar unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Crie um novo unifiedRoleAssignment postando na coleção roleAssignment. |
| [Excluir unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | Nenhum | Exclua o objeto unifiedRoleAssignment. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador exclusivo do unifiedRoleAssignment. Chave, não anulada, somente leitura. |
|roleDefinitionId|String| Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. Suporta `$filter` (`eq` somente operador). |
|principalId|String| Identificador da entidade à qual a atribuição é concedida. Suporta `$filter` (`eq` somente operador). |
|directoryScopeId|String|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|appScopeId|String|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.  Para o provedor de gerenciamento de direitos, use escopos de aplicativo para especificar um catálogo, por exemplo `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997`.|
|resourceScope|String| O escopo no qual o unifiedRoleAssignment se aplica. Isso é `/` para todo o serviço. **NÃO USE. Essa propriedade será preterida em breve.**|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|appScope|[appScope](appscope.md)|Detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
|directoryScope|[directoryObject](directoryobject.md)|O objeto directory que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função. Somente leitura. Oferece suporte para `$expand`. |
|principal|[directoryObject](directoryobject.md)| A entidade atribuída. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Oferece suporte para `$expand`. |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|A funçãoDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. **roleDefinition.id** será expandido automaticamente. Suporta o `$expand`. |



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
