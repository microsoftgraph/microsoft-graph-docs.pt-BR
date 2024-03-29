---
title: Tipo de recurso iosLobAppProvisioningConfigurationAssignment
description: Uma classe que contém as propriedades usadas para a atribuição de grupo de um provisionamento e configuração de aplicativos LOB do iOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30fb0252a8dadf081c6b016a538343c07589c1c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054594"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>Tipo de recurso iosLobAppProvisioningConfigurationAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a atribuição de grupo de um provisionamento e configuração de aplicativos LOB do iOS.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosLobAppProvisioningConfigurationAssignments](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|[Coleção iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Listar propriedades e relações dos [objetos iosLobAppProvisioningConfigurationAssignment.](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|
|[Obter iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Leia propriedades e relações do [objeto iosLobAppProvisioningConfigurationAssignment.](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|
|[Criar iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Crie um novo [objeto iosLobAppProvisioningConfigurationAssignment.](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|
|[Excluir iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|Nenhum|Exclui um [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).|
|[Atualizar iosLobAppProvisioningConfigurationAssignment](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|Atualize as propriedades de [um objeto iosLobAppProvisioningConfigurationAssignment.](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



