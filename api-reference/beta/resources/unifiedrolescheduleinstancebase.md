---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Propriedade base da instância de agendamento de função unificada que combina instância de agendamento de atribuição de função unificada e instância de agendamento de qualificação de função unificada
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ddf4311fdddc44089410a0f073d6e041660283f2
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682198"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

"Propriedade base da instância de agendamento de função unificada que combina instância de agendamento de atribuição de função unificada e instância de agendamento de qualificação de função unificada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|String|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|directoryScopeId|String|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.|
|id|String|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulada, somente leitura.|
|principalId|String|Objectid da entidade à qual a atribuição está sendo concedida.|
|roleDefinitionId|String|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura.|

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
