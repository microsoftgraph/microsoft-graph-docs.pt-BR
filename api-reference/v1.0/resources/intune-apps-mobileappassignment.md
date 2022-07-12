---
title: Tipo de recurso mobileAppAssignment
description: Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6513793cae2dc77807cc20940e14f1421d53122d
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732461"
---
# <a name="mobileappassignment-resource-type"></a>Tipo de recurso mobileAppAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppAssignments](../api/intune-apps-mobileappassignment-list.md)|Conjunto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Listar propriedades e relações de objetos de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Obter mobileAppAssignment](../api/intune-apps-mobileappassignment-get.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Ler propriedades e relações de objetos de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Criar mobileAppAssignment](../api/intune-apps-mobileappassignment-create.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Criar um novo objeto de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Excluir mobileAppAssignment](../api/intune-apps-mobileappassignment-delete.md)|Nenhum|Excluir uma [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|
|[Atualizar mobileAppAssignment](../api/intune-apps-mobileappassignment-update.md)|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Atualizar as propriedades de um objeto de [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|finalidade|[installIntent](../resources/intune-shared-installintent.md)|A finalidade da instalação definida pelo administrador. Os valores possíveis são: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A atribuição do grupo de destino definida pelo administrador.|
|configurações|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|As configurações para a atribuição de destino definida pelo administrador.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings",
    "notifications": "String",
    "restartSettings": {
      "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
      "gracePeriodInMinutes": 1024,
      "countdownDisplayBeforeRestartInMinutes": 1024,
      "restartNotificationSnoozeDurationInMinutes": 1024
    },
    "installTimeSettings": {
      "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
      "useLocalTime": true,
      "startDateTime": "String (timestamp)",
      "deadlineDateTime": "String (timestamp)"
    },
    "deliveryOptimizationPriority": "String"
  }
}
```





