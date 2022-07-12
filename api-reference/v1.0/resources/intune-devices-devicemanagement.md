---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 767292c6606294f383487f4aff4f20eda5f20f1f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66720763"
---
# <a name="devicemanagement-resource-type"></a>Tipo de recurso deviceManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagement](../api/intune-devices-devicemanagement-get.md)|[deviceManagement](../resources/intune-devices-devicemanagement.md)|Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-devices-devicemanagement.md).|
|[Atualizar deviceManagement](../api/intune-devices-devicemanagement-update.md)|[deviceManagement](../resources/intune-devices-devicemanagement.md)|Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-devices-devicemanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|Estado de assinatura de gerenciamento de dispositivo móvel do locatário. Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Certificado de notificação por push da Apple.|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|Visão geral do dispositivo|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|A lista de aplicativos detectados associados a um dispositivo.|
|managedDevices|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|A lista de dispositivos gerenciados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```





