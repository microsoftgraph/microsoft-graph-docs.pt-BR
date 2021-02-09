---
title: Tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de serviço em um escopo específico para fins de concessão de acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4df17c6b112cefe03a12631ee763f49e976fb568
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159840"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>Tipo de recurso unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos. Ele representa uma definição de função atribuída a uma matriz de entidades de segurança (normalmente um usuário) em uma matriz de escopo. Um exemplo desse provedor de RBAC é o Microsoft Intune. No Microsoft Intune, você pode criar uma atribuição de função com várias entidades e vários escopos.

É necessário **fornecer directoryScopeIds** ou **appScopeIds.**

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Ler propriedades e relações do objeto unifiedRoleAssignmentMultiple. |
| [Criar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment. |
| [Atualizar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Atualize um objeto unifiedRoleAssignmentMultiple existente. |
| [Excluir unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | Nenhum(a) | Exclua o objeto unifiedRoleAssignmentMultiple. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | String | O identificador exclusivo do unifiedRoleAssignmentMultiple. Chave, não anulada, somente leitura. |
| displayName | String | Nome da atribuição de função. Obrigatório. |
| description | String | Descrição da atribuição de função. |
| roleDefinitionId | String | ID do unifiedRoleDefinition para o que a atribuição se destina. |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |Propriedade que indica a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que a atribuição de função. Somente leitura.  |
| principalIds | Coleção de cadeias de caracteres | Objectids das entidades às quais a atribuição é concedida. |
| entidades de| Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência às entidades atribuídas. Fornecido para que os chamadores possam obter as entidades de `$expand` serviço usando ao mesmo tempo que a atribuição de função. Somente leitura. |
| directoryScopeIds | Coleção de cadeias de caracteres | IDs dos objetos de diretório que representam os escopos da atribuição. Os escopos de uma atribuição determinam o conjunto de recursos para os quais as entidades foram concedidas acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. |
| directoryScopes | Coleção [directoryObject](directoryobject.md) | Coleção somente leitura fazendo referência aos objetos de diretório que são escopo da atribuição. Fornecido para que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que a atribuição de função. Somente leitura. |
| appScopeIds | Coleção de cadeias de caracteres | IDs dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Os escopos de uma atribuição determinam o conjunto de recursos para os quais a entidade de serviço recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para escopo em todo o locatário. Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. |
| appScopes | [Coleção appScope](appscope.md) |Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo. Entidade de contenção. Somente leitura.  |

## <a name="relationships"></a>Relações

Nenhum

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


