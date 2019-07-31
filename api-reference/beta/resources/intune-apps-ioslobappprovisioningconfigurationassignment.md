---
title: tipo de recurso iosLobAppProvisioningConfigurationAssignment
description: Uma classe que contém as propriedades usadas para atribuição de grupo de um provisionamento e configuração de aplicativos LOB iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ad185eebd1cf74dfcdf35ec3a8b9fa46fb7ea5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005944"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>tipo de recurso iosLobAppProvisioningConfigurationAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para atribuição de grupo de um provisionamento e configuração de aplicativos LOB iOS.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosLobAppProvisioningConfigurationAssignments](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|coleção [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Listar Propriedades e relações dos objetos [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Obter iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Leia as propriedades e as relações do objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Criar iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Criar um novo objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|
|[Excluir iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|Nenhum|Exclui [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).|
|[Atualizar iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Atualiza as propriedades de um objeto [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|A atribuição do grupo de destino definida pelo administrador.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





