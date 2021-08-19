---
title: tipo de recurso userExperienceAnalyticsAppHealthDevicePerformance
description: A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes de desempenho do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1197f69ee9b4279332c73a83e841306593280b03
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266188"
---
# <a name="userexperienceanalyticsapphealthdeviceperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes de desempenho do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-list.md)|[coleção userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Obter userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-get.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Criar userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-create.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|
|[Excluir userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-update.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do dispositivo de análise de experiência do usuário.|
|deviceModel|Cadeia de caracteres|O nome do modelo do dispositivo.|
|deviceManufacturer|Cadeia de caracteres|O nome do fabricante do dispositivo.|
|appCrashCount|Int32|O número de falhas de aplicativo para o dispositivo. Valores válidos -2147483648 para 2147483647|
|crashedAppCount|Int32|O número de falhas distintas do aplicativo para o dispositivo. Valores válidos -2147483648 para 2147483647|
|appHangCount|Int32|O número de travas de aplicativo para o dispositivo. Valores válidos -2147483648 para 2147483647|
|processedDateTime|DateTimeOffset|A data e a hora em que as estatísticas foram computadas pela última vez.|
|meanTimeToFailureInMinutes|Int32|O tempo de falha média do dispositivo em minutos. Valores válidos -2147483648 para 2147483647|
|deviceAppHealthScore|Duplo|A pontuação de saúde do aplicativo do dispositivo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|deviceAppHealthStatus|Cadeia de caracteres|O status geral da saúde do aplicativo do dispositivo.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
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
  "processedDateTime": "String (timestamp)",
  "meanTimeToFailureInMinutes": 1024,
  "deviceAppHealthScore": "4.2",
  "deviceAppHealthStatus": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```




