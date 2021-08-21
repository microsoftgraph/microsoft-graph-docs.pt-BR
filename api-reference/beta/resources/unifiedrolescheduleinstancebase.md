---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Propriedade base da instância de agendamento de função unificada que combina instância de agendamento de atribuição de função unificada e instância de agendamento de qualificação de função unificada
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 56d05213ae5088d4b0088deb21042c1bfc5d0540
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453909"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

Propriedade base da instância de agendamento de função unificada que combina instâncias de agendamento de atribuição de função unificada e instâncias de agendamento de qualificação de função unificada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. |
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. |
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulada, somente leitura.|
|principalId|Cadeia de caracteres|Identificador da entidade à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. |
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. <br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. |
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto directory que é o escopo da atribuição. Habilita a recuperação do objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função. Apenas leitura.|
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
