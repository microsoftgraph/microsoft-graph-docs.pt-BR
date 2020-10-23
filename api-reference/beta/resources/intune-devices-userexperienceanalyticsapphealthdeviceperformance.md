---
title: tipo de recurso userExperienceAnalyticsAppHealthDevicePerformance
description: A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e7a7775edf7893aeaefa75fc507b930cc8a5234
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733970"
---
# <a name="userexperienceanalyticsapphealthdeviceperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-list.md)|coleção [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Obter userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-get.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Criar userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-create.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|
|[Excluir userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-update.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.|
|deviceModel|Cadeia de caracteres|O nome do modelo do dispositivo.|
|deviceManufacturer|String|O nome do fabricante do dispositivo.|
|appCrashCount|Int32|O número de falhas do aplicativo para o dispositivo. Valores válidos-2147483648 a 2147483647|
|crashedAppCount|Int32|O número de falhas de aplicativos distintos para o dispositivo. Valores válidos-2147483648 a 2147483647|
|appHangCount|Int32|O número de bloqueios de aplicativo para o dispositivo. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo médio de falha para o dispositivo em minutos. Valores válidos-2147483648 a 2147483647|
|deviceAppHealthScore|Duplo|A pontuação de integridade do aplicativo do dispositivo. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|deviceAppHealthStatus|String|O status de integridade geral do aplicativo do dispositivo.|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|deviceDisplayName|Cadeia de caracteres|O nome do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "appCrashCount": 1024,
  "crashedAppCount": 1024,
  "appHangCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "deviceAppHealthScore": "4.2",
  "deviceAppHealthStatus": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```





