---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Um modelo que expõe propriedades e relações usadas nos tipos de recurso unifiedRoleAssignmentScheduleInstance e unifiedRoleEligibilityScheduleInstance.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a5248cfe962dbaf75b19ae3777a3d6a35f70e37e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898697"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

Um modelo que expõe propriedades e relações usadas nos tipos de recurso [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md) e [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md) .


Herda de [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de Caracteres|Identificador do escopo específico do aplicativo quando a atribuição ou a elegibilidade de função estiver no escopo de um aplicativo. O escopo de uma atribuição ou elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|directoryScopeId|Cadeia de Caracteres|Identificador do objeto de diretório que representa o escopo da atribuição ou qualificação de função. O escopo de uma atribuição ou elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|String|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md).|
|principalId|Cadeia de Caracteres|Identificador da entidade de segurança que recebeu a atribuição de função ou que está qualificado para uma função.|
|roleDefinitionId|Cadeia de Caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança ou para o qual a entidade de segurança está qualificada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a atribuição ou a elegibilidade de função estiver no escopo de um aplicativo. Anulável.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição ou elegibilidade de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma atribuição de função ou elegibilidade de função por meio da solicitação.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** .|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "baseType": "microsoft.graph.entity",
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