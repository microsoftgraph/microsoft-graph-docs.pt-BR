---
title: Tipo de recurso mobileAppAssignment
description: Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a369dbc55e7b3736fcb811fb3212cea20bf889d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790877"
---
# <a name="mobileappassignment-resource-type"></a>Tipo de recurso mobileAppAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe com as propriedades usadas para atribuição de grupos de um aplicativo móvel.

## <a name="methods"></a>Methods
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
|configurações|[mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)|As configurações para a atribuição de destino definida pelo administrador.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|O tipo de recurso que é a origem da atribuição. Os valores possíveis são: `direct` e `policySets`.|
|sourceId|String|O identificador da origem da atribuição.|

## <a name="relationships"></a>Relações
Nenhuma

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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "settings": {
    "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
    "vpnConfigurationId": "String",
    "uninstallOnDeviceRemoval": true
  },
  "source": "String",
  "sourceId": "String"
}
```



