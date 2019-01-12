---
title: tipo de recurso de deviceConfigurationTargetedUserAndDevice
description: Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947958"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>tipo de recurso de deviceConfigurationTargetedUserAndDevice

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Resumo de um conjunto de políticas de configuração de dispositivo de conflito.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceId|Cadeia de caracteres|A id do dispositivo em que o check-in.|
|deviceName|Cadeia de caracteres|O nome do dispositivo em que o check-in.|
|userId|Cadeia de caracteres|A identificação do usuário no check-in.|
|userDisplayName|Cadeia de caracteres|O nome de exibição do usuário no check-in|
|userPrincipalName|Cadeia de caracteres|O UPN do usuário no check-in.|
|lastCheckinDateTime|DateTimeOffset|Última hora de check-in para este par de dispositivo do usuário.|

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





