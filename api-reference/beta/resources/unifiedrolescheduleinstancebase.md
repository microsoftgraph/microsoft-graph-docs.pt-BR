---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Propriedade base da instância de agendamento de função unificada que combina instância de agendamento de atribuição de função unificada e instância de agendamento de qualificação de função unificada
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4f22af61c513f8cc559948fb5519af5ac903d1d7c4ed650d2d11c6f5bf665282
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238941"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

"Propriedade base da instância de agendamento de função unificada que combina instância de agendamento de atribuição de função unificada e instância de agendamento de qualificação de função unificada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|directoryScopeId|Cadeia de caracteres|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulada, somente leitura.|
|principalId|Cadeia de caracteres|Objectid da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto directory que é o escopo da atribuição. Habilita a recuperação do objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade que está recebendo uma atribuição de função por meio da solicitação. Habilita a recuperação da entidade principal usando `$expand` ao mesmo tempo que obter a atribuição de função. Somente leitura.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|A funçãoDefinition para a atribuição. Habilita a recuperação da definição de função usando `$expand` ao mesmo tempo que obter a atribuição de função. O roleDefinition.Id é expandido automaticamente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleScheduleInstanceBase",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String"
}
```
