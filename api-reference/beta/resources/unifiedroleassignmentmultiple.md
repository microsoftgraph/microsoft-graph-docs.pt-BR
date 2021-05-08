---
title: Tipo de recurso unifiedRoleAssignmentMultiple
description: Uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) sobre uma matriz de escopo.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b6f345dbf4947212f22a5386fded551d62b0e24d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241055"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>Tipo de recurso unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos. Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) sobre uma matriz de escopo. Um exemplo desse provedor RBAC é Microsoft Intune. Em Microsoft Intune, você pode criar uma atribuição de função com várias entidades principais e vários escopos.

É necessário **fornecer directoryScopeIds** **ou appScopeIds.**

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar UnifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-list.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Leia uma lista de objetos unifiedRoleAssignmentMultiple e suas propriedades. |
| [Obter unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Ler propriedades e relações do objeto unifiedRoleAssignmentMultiple. |
| [Criar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment. |
| [Atualizar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Atualize um objeto unifiedRoleAssignmentMultiple existente. |
| [Excluir unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Nenhum | Exclua o objeto unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | Cadeia de caracteres | O identificador exclusivo do unifiedRoleAssignmentMultiple. Chave, não anulada, somente leitura. |
| displayName | Cadeia de caracteres | Nome da atribuição de função. Obrigatório. |
| description | Cadeia de caracteres | Descrição da atribuição de função. |
| roleDefinitionId | Cadeia de caracteres | Identificador do unifiedRoleDefinition para o que a atribuição se destina. |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Suporta `$filter` ( operador em `eq` **id,** **isBuiltIn** e **displayName** e `startsWith` operador em **displayName**) e `$expand` .  |
| principalIds | Coleção de cadeias de caracteres | Identificadores das entidades a que a atribuição é concedida.  Suporta `$filter` ( `any` somente operador). |
| directoryScopeIds | Coleção de cadeias de caracteres | Ids dos objetos de diretório que representam os escopos da atribuição. Os escopos de uma atribuição determinam o conjunto de recursos para os quais as entidades foram concedidas acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |
| appScopeIds | Coleção de cadeias de caracteres | Ids dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Os escopos de uma atribuição determinam o conjunto de recursos para os quais a entidade recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| appScopes | [Coleção appScope](appscope.md) |Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Entidade de contenção. Somente leitura.  |
| directoryScopes | Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência aos objetos de diretório que são escopo da atribuição. Fornecido para que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura.  Oferece suporte para `$expand`.|
| principais| Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência às entidades atribuídas. Fornecido para que os chamadores possam obter as entidades que `$expand` usam ao mesmo tempo que obter a atribuição de função. Somente leitura.  Oferece suporte para `$expand`.|
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|A funçãoDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. **roleDefinition.id** será expandido automaticamente. Oferece suporte para `$expand`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


