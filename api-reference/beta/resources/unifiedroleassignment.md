---
title: tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 683a6daf510e10c53cf44ec64d93ce2398212ce4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218034"
---
# <a name="unifiedroleassignment-resource-type"></a>tipo de recurso unifiedRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignment é usado para conceder acesso aos recursos. Ele representa uma definição de função atribuída a uma entidade de segurança (normalmente um usuário) em um determinado escopo.

O fornecimento de um directoryScopeId ou um appScopeId é necessário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignment. |
| [Criar unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Crie um novo unifiedRoleAssignment postando na coleção roleAssignment. |
| [Excluir unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | None | Exclua o objeto unifiedRoleAssignment. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador exclusivo para o unifiedRoleAssignment. Chave, não anulável, somente leitura. |
|roleDefinitionId|Cadeia de Caracteres| ID do unifiedRoleDefinition para o qual a atribuição é. Somente leitura. |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|Propriedade que indica o roleDefinition para o qual a atribuição é. Fornecido de modo que os chamadores possam obter a definição `$expand` de função usando ao mesmo tempo em que se obtém a atribuição de função. roleDefinition.Id será expandido automaticamente
|principalId|Cadeia de Caracteres| ObjectID da entidade de segurança para a qual a atribuição é concedida. |
|requere|[directoryObject](directoryobject.md)| Propriedade que faz referência à entidade de segurança atribuída. Desde que os chamadores possam obter a entidade de `$expand` segurança usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
|directoryScopeId|Cadeia de Caracteres|ID do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.|
|directoryScope|[directoryObject](directoryobject.md)|Propriedade fazendo referência ao objeto Directory que é o escopo da atribuição. Fornecido de modo que os chamadores possam obter o objeto `$expand` de diretório usando ao mesmo tempo em que se obtém a atribuição de função. Somente leitura. |
|appScopeId|Cadeia de Caracteres|ID do escopo específico do aplicativo quando o escopo da atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para escopo em todo o locatário. Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.|
|appScope|[appScope](appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo da atribuição é específico de aplicativo. Entidade de confinamento. |
|resourceScope|Cadeia de Caracteres| O escopo no qual o unifiedRoleAssignment se aplica. Isso é "/" para todo o serviço. **NÃO USE. Essa propriedade será preterida em breve.**|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
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