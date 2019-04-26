---
title: tipo de recurso deviceConfigurationTargetedUserAndDevice
description: Resumo de conflito para um conjunto de políticas de configuração de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2ddd31671f8cd277dbc7390c8c561189b6c0e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567260"
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





