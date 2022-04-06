---
title: Tipo de recurso unifiedRoleScheduleBase
description: Propriedade base de agendamentos de função unificada que combina agendas de atribuição de função unificada e agendas de qualificação de função unificada
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b7c93dfcec24db531e7ae61924dda3e84695d3
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510145"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Propriedade base de agendamentos de função unificada que combina agendas de atribuição de função unificada e agendas de qualificação de função unificada

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo           | Descrição               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | String         | Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas ou todos os usuários. |
| createdDateTime  | DateTimeOffset | Hora em que a agenda foi criada. |
| createdUsing     | Cadeia de caracteres         | Identificador da roleAssignmentScheduleRequest que criou essa agenda. |
| directoryScopeId | Cadeia de caracteres         | Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. |
| id               | Cadeia de caracteres         | O identificador exclusivo para unifiedRoleAssignmentSchedule. Chave, não anulada, somente leitura. |
| modifiedDateTime | DateTimeOffset | Última vez que a agenda foi atualizada. |
| principalId      | Cadeia de caracteres         | Identificador da entidade à qual a atribuição está sendo concedida. Suporta `$filter` (`eq`). |
| roleDefinitionId | String         | Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. Suporta `$filter` (`eq`). |
| status           | Cadeia de caracteres         | Status do `roleAssignmentSchedule`. Pode incluir mensagens relacionadas ao estado, `Provisioned`como , `Revoked`, `Pending Provisioning`e `Pending Approval`. Suporta `$filter` (`eq`).  |

## <a name="relationships"></a>Relações

| Relação   | Tipo                                                                               | Descrição               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (Preterido) | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Depreciado. |
| appScope       | [appScope](../resources/appscope.md)                                               | Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função. Somente leitura. |
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
