---
title: Tipo de recurso unifiedRoleScheduleBase
description: Propriedade base de agendamentos de função unificada que combina agendas de atribuição de função unificada e agendas de qualificação de função unificada
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 898f990ae7ffa09b3f251ce83fd71da04c2eafc6
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298993"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleBase

Namespace: microsoft.graph

Propriedade base de agendamentos de função unificada que combina agendas de atribuição de função unificada e agendas de qualificação de função unificada

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo           | Descrição               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | Cadeia de caracteres         | ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |
| createdDateTime  | DateTimeOffset | Hora em que a agenda foi criada. |
| createdUsing     | Cadeia de caracteres         | ID da roleAssignmentScheduleRequest que criou essa agenda. |
| directoryScopeId | Cadeia de caracteres         | ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. |
| id               | Cadeia de caracteres         | O identificador exclusivo para unifiedRoleAssignmentSchedule. Chave, não anulada, somente leitura. |
| modifiedDateTime | DateTimeOffset | Última vez que a agenda foi atualizada. |
| principalId      | Cadeia de caracteres         | Objectid da entidade à qual a atribuição está sendo concedida. |
| roleDefinitionId | Cadeia de caracteres         | ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. |
| status           | Cadeia de caracteres         | Status do `roleAssignmentSchedule` . Pode incluir mensagens relacionadas ao `Provisioned` estado, `Revoked` como , , `Pending Provisioning` e `Pending Approval` . |

## <a name="relationships"></a>Relações

| Relação   | Tipo                                                                               | Descrição               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Será preterido. |
| appScope       | [appScope](../resources/appscope.md)                                               | Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
| principal      | [directoryObject](../resources/directoryobject.md)                                 | Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String"
}
```
