---
title: Tipo de recurso unifiedRoleScheduleInstanceBase
description: Um modelo que expõe propriedades e relações usadas nos tipos de recurso unifiedRoleAssignmentScheduleInstance e unifiedRoleEligibilityScheduleInstance.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 241c0af15867d87775490e00bd0f098e13e9dd9a
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133960"
---
# <a name="unifiedrolescheduleinstancebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleInstanceBase

Namespace: microsoft.graph

Um modelo que expõe propriedades e relações usadas nos tipos de recurso [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md) e [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md) .


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum. 

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleInstanceBases](../api/unifiedrolescheduleinstancebase-list.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection|Get a list of the [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) objects and their properties.|
|[Get unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-get.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Read the properties and relationships of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Update unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-update.md)|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Update the properties of an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[Delete unifiedRoleScheduleInstanceBase](../api/unifiedrolescheduleinstancebase-delete.md)|None|Deletes an [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) object.|
|[List appScope](../api/unifiedrolescheduleinstancebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedrolescheduleinstancebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedrolescheduleinstancebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedrolescheduleinstancebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedrolescheduleinstancebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedrolescheduleinstancebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedrolescheduleinstancebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
-->

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a atribuição ou a elegibilidade de função estiver no escopo de um aplicativo. O escopo de uma atribuição ou elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição ou qualificação de função. O escopo de uma atribuição ou elegibilidade de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a atribuição de função ou que está qualificado para uma função.|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança ou para o qual a entidade de segurança está qualificada.|

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

