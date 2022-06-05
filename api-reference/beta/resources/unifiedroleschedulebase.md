---
title: Tipo de recurso unifiedRoleScheduleBase
description: Um modelo que expõe propriedades e relações usadas nos tipos de recursos unifiedRoleAssignmentSchedule e unifiedRoleEligibilitySchedule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e422b4b30da252c028003abd35134ea1c06874e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898333"
---
# <a name="unifiedroleschedulebase-resource-type"></a>Tipo de recurso unifiedRoleScheduleBase

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um modelo que expõe propriedades e relações usadas nos tipos de recursos [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) e [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) .


Herda de [entidade](../resources/entity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de Caracteres|Identificador do escopo específico do aplicativo quando a atribuição ou a elegibilidade está no escopo de um aplicativo. O escopo de uma atribuição ou qualificação determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas.|
|createdDateTime|DateTimeOffset|Quando a agenda foi criada.|
|createdUsing|Cadeia de Caracteres|Identificador do objeto por meio do qual essa agenda foi criada.|
|directoryScopeId|Cadeia de Caracteres|Identificador do objeto de diretório que representa o escopo da atribuição ou qualificação. O escopo de uma atribuição ou qualificação determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo.|
|id|String|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|Quando a agenda foi modificada pela última vez.|
|principalId|Cadeia de Caracteres|Identificador da entidade de segurança que recebeu a atribuição de função ou a qualificação.|
|roleDefinitionId|Cadeia de Caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança ou para o qual uma entidade de segurança está qualificada.|
|status|String|O status da atribuição de função ou da solicitação de qualificação.|

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