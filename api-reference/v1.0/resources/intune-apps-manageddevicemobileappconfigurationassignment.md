---
title: Tipo de recurso managedDeviceMobileAppConfigurationAssignment
description: Contém as propriedades usadas para atribuir uma configuração de aplicativo MDM a um grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54754ad74a93788c9eab83ae30950d1f76d84c87
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118492"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a>Tipo de recurso managedDeviceMobileAppConfigurationAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades usadas para atribuir uma configuração de aplicativo MDM a um grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceMobileAppConfigurationAssignments](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|Conjunto [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Listar propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Obter managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Criar managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Criar um novo objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Excluir managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|Nenhum|Excluir um [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Atualizar managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao qual a política de T&C foi designada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  }
}
```




