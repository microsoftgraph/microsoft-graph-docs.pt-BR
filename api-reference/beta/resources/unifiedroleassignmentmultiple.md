---
title: Tipo de recurso unifiedRoleAssignmentMultiple
description: Uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) sobre uma matriz de escopo.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7db7ababef04111146c4a39c3dc6550339e67d3a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533882"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>Tipo de recurso unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos, como [](rolemanagement.md)parte do Microsoft 365 de função RBAC . Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) sobre uma matriz de escopos. 

Você pode criar uma atribuição de função com várias entidades principais e vários escopos.

Você deve fornecer **directoryScopeIds** ou **appScopeIds**.

No momento, há suporte para os seguintes provedores RBAC:
- Cloud PC 
- Microsoft Intune

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md) | [Coleção unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Leia uma lista de objetos unifiedRoleAssignmentMultiple e suas propriedades. |
| [Criar unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment. |
| [Obter unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Ler propriedades e relações do objeto unifiedRoleAssignmentMultiple. |
| [Atualizar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Atualize um objeto unifiedRoleAssignmentMultiple existente. |
| [Excluir unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Nenhum | Exclua o objeto unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| appScopeIds | Coleção de cadeias de caracteres | Ids dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Os escopos de uma atribuição determinam o conjunto de recursos para os quais a entidade recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |
| description | String | Descrição da atribuição de função. |
| directoryScopeIds | Coleção de cadeias de caracteres | Ids dos objetos de diretório que representam os escopos da atribuição. Os escopos de uma atribuição determinam o conjunto de recursos para os quais as entidades foram concedidas acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |
| displayName | String | Nome da atribuição de função. Obrigatório. |
| id | String | O identificador exclusivo do unifiedRoleAssignmentMultiple. Chave, não anulada, somente leitura. |
| roleDefinitionId | Cadeia de Caracteres | Identificador do unifiedRoleDefinition para o que a atribuição se destina. |
| principalIds | Coleção de cadeias de caracteres | Identificadores das entidades a que a atribuição é concedida.  Suporta `$filter` ( `any` somente operador). |


## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| appScopes | [Coleção appScope](appscope.md) |Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Entidade de contenção. Somente leitura.  |
| directoryScopes | Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência aos objetos de diretório que são escopo da atribuição. Fornecido para que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura.  Oferece suporte para `$expand`.|
| principais| Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência às entidades atribuídas. Fornecido para que os chamadores possam obter as entidades que `$expand` usam ao mesmo tempo que obter a atribuição de função. Somente leitura.  Oferece suporte para `$expand`.|
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Especifica a funçãoDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função.  Suporta `$filter` ( operador em `eq` **id,** **isBuiltIn** e **displayName** e `startsWith` operador em **displayName**) e `$expand` . |


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


