---
title: Tipo de recurso unifiedRoleScheduleBase
description: Um modelo que expõe propriedades e relações usadas nos tipos de recursos unifiedRoleAssignmentSchedule e unifiedRoleEligibilitySchedule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9f778ac684ddb0ef9ae04647c4aa12193dff919c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133951"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleBase

Namespace: microsoft.graph

Um modelo que expõe propriedades e relações usadas nos tipos de recursos [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) e [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) .


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum.

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleScheduleBases](../api/unifiedroleschedulebase-list.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection|Get a list of the [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) objects and their properties.|
|[Get unifiedRoleScheduleBase](../api/unifiedroleschedulebase-get.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Read the properties and relationships of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Update unifiedRoleScheduleBase](../api/unifiedroleschedulebase-update.md)|[unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|Update the properties of an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[Delete unifiedRoleScheduleBase](../api/unifiedroleschedulebase-delete.md)|None|Deletes an [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) object.|
|[List appScope](../api/unifiedroleschedulebase-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScope navigation property.|
|[Add appScope](../api/unifiedroleschedulebase-post-appscope.md)|[appScope](../resources/appscope.md)|Add appScope by posting to the appScope collection.|
|[List directoryScope](../api/unifiedroleschedulebase-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedroleschedulebase-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[List principal](../api/unifiedroleschedulebase-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principal navigation property.|
|[Add principal](../api/unifiedroleschedulebase-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[List unifiedRoleDefinition](../api/unifiedroleschedulebase-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinition resources from the roleDefinition navigation property.|
|[Add unifiedRoleDefinition](../api/unifiedroleschedulebase-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|

-->

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a atribuição ou a elegibilidade está no escopo de um aplicativo. O escopo de uma atribuição ou qualificação determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|createdDateTime|DateTimeOffset|Quando a agenda foi criada.|
|createdUsing|Cadeia de caracteres|Identificador do objeto por meio do qual essa agenda foi criada.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição ou qualificação. O escopo de uma atribuição ou qualificação determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|Quando a agenda foi modificada pela última vez.|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a atribuição de função ou a qualificação.|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança ou para o qual uma entidade de segurança está qualificada.|
|status|Cadeia de caracteres|O status da atribuição de função ou da solicitação de qualificação.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a atribuição ou qualificação de função está no escopo de um aplicativo. Anulável.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição ou qualificação de função. Somente leitura.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está recebendo uma atribuição de função ou que está qualificada para uma função por meio da solicitação.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** .|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleScheduleBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
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

