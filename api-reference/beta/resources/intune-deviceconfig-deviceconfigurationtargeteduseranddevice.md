---
title: tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 632f371c6db6c962b20e36d50c33ad2e883bc774
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004551"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>tipo de recurso deviceConfigurationTargetedUserAndDevice

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo de conflito para um conjunto de políticas de configuração de dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceId|Cadeia de caracteres|A ID do dispositivo no check-in.|
|deviceName|String|O nome do dispositivo no check-in.|
|userId|String|A ID do usuário no check-in.|
|userDisplayName|String|O nome de exibição do usuário no check-in|
|userPrincipalName|String|O UPN do usuário no check-in.|
|lastCheckinDateTime|DateTimeOffset|Horário da última verificação para este par de usuários/dispositivos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





