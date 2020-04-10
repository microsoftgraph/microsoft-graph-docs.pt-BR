---
title: tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20e0d7a213ea6e46db9cf9774c46bda0070ecd27
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218027"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>tipo de recurso unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos. Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) em uma matriz de escopo. Um exemplo de um provedor RBAC é o Microsoft Intune. No Microsoft Intune, você pode criar uma atribuição de função com várias entidades e vários escopos.

É necessário fornecer o **directoryScopeIds** ou o **appScopeIds** .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignmentMultiple. |
| [Criar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment. |
| [Atualizar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Atualize um objeto unifiedRoleAssignmentMultiple existente. |
| [Excluir unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | None | Exclua o objeto unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | String | O identificador exclusivo para o unifiedRoleAssignmentMultiple. Chave, não anulável, somente leitura. |
| displayName | Cadeia de caracteres | Nome da atribuição de função. |
| description | String | Descrição da atribuição de função. |
| roleDefinitionId | Cadeia de Caracteres | ID do unifiedRoleDefinition para o qual a atribuição é. Somente leitura. |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Propriedade que indica o roleDefinition para o qual a atribuição é. Fornecido de modo que os chamadores possam obter a definição `$expand` de função usando ao mesmo tempo em que se obtém a atribuição de função. |
| principalIds | Coleção de cadeias de caracteres | ObjectIDs das entidades de segurança para as quais a atribuição é concedida. |
| entidades| Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência a entidades de segurança atribuídas. Desde que os chamadores possam obter as entidades usando `$expand` ao mesmo tempo em que se obtém a atribuição de função. Somente leitura. |
| directoryScopeIds | Coleção de cadeias de caracteres | IDs dos objetos de diretório que representam os escopos da atribuição. Os escopos de uma atribuição determinam o conjunto de recursos para o qual foram concedidos acesso a entidades de segurança. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas. |
| directoryScopes | Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência aos objetos de diretório que são o escopo da atribuição. Desde que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
| appScopeIds | Coleção de cadeias de caracteres | IDs dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Os escopos de uma atribuição determinam o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para escopo em todo o locatário. Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas. |
| appScopes | coleção [appScope](appscope.md) |Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Entidade de confinamento. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
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