---
title: Tipo de recurso unifiedRoleScheduleBase
description: Propriedade base de agendas de função unificada que combina agendas unificadas de atribuição de função e agendas de qualificação de função unificada
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dbe8b597286bacd9c6f8d0a7dc17cf82296fadb9
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398830"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Propriedade base de agendas de função unificada que combina agendas unificadas de atribuição de função e agendas de qualificação de função unificada

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo           | Descrição               |
| :--------------- | :------------- | :------------------------ |
| appScopeId       | Cadeia de caracteres         | Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas ou todos os usuários. |
| createdDateTime  | DateTimeOffset | Hora em que a agenda foi criada. |
| createdUsing     | Cadeia de caracteres         | Identificador da roleAssignmentScheduleRequest que criou esse agendamento. |
| directoryScopeId | Cadeia de caracteres         | Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. |
| id               | Cadeia de caracteres         | O identificador exclusivo para unifiedRoleAssignmentSchedule. Chave, não anulável, somente leitura. |
| modifiedDateTime | DateTimeOffset | Última vez em que o agendamento foi atualizado. |
| principalId      | Cadeia de caracteres         | Identificador da entidade de segurança à qual a atribuição está sendo concedida. Suporta `$filter` (`eq`). |
| roleDefinitionId | Cadeia de caracteres         | Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura. Suporta `$filter` (`eq`). |
| status           | Cadeia de caracteres         | Status do `roleAssignmentSchedule`. Ele pode incluir mensagens relacionadas ao estado `Provisioned`, `Revoked`como , `Pending Provisioning`e `Pending Approval`. Suporta `$filter` (`eq`).  |

## <a name="relationships"></a>Relações

| Relação   | Tipo                                                                               | Descrição               |
| :------------- | :--------------------------------------------------------------------------------- | :------------------------ |
| activeInstance (preterido) | [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) | Depreciado. |
| appScope       | [appScope](../resources/appscope.md)                                               | Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
| directoryScope | [directoryObject](../resources/directoryobject.md)                                 | Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
| principal      | [directoryObject](../resources/directoryobject.md)                                 | Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade de segurança `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. |
| roleDefinition | [unifiedRoleDefinition](../resources/unifiedroledefinition.md)                     | Propriedade que indica a roleDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente. |

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
