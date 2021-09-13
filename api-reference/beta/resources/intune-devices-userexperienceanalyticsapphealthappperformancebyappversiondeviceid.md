---
title: Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
description: A entidade de desempenho do aplicativo de análise de experiência do usuário contém o desempenho do aplicativo por ID do dispositivo de versão do aplicativo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a730dc54bcd7095f21bf503cbf341dfd66187880
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081049"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversiondeviceid-resource-type"></a>Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise de experiência do usuário contém o desempenho do aplicativo por ID do dispositivo de versão do aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceIds](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-list.md)|[coleção userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Obter userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|
|[Excluir userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md).|
|[Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceDisplayName|Cadeia de caracteres|O nome do dispositivo.|
|processedDateTime|DateTimeOffset|A data e a hora em que as estatísticas foram computadas pela última vez.|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo.|
|appPublisher|Cadeia de Caracteres|O editor do aplicativo.|
|appVersion|Cadeia de caracteres|A versão do aplicativo.|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceDisplayName": "String",
  "processedDateTime": "String (timestamp)",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "appCrashCount": 1024
}
```



