---
title: Tipo de recurso userExperienceAnalyticsResourcePerformance
description: A entidade de desempenho do recurso de análise de experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9d2434ef45b0032b9d606dae7715213844c06e50
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786968"
---
# <a name="userexperienceanalyticsresourceperformance-resource-type"></a>Tipo de recurso userExperienceAnalyticsResourcePerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do recurso de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsResourcePerformances](../api/intune-devices-userexperienceanalyticsresourceperformance-list.md)|[coleção userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Obter userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-get.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Criar userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-create.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Crie um novo [objeto userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[Excluir userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md).|
|[Atualizar userExperienceAnalyticsResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-update.md)|[userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsResourcePerformance.](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|
|[função summarizeDeviceResourcePerformance](../api/intune-devices-userexperienceanalyticsresourceperformance-summarizedeviceresourceperformance.md)|[coleção userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da entidade de desempenho do recurso de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceName|String|O nome do dispositivo.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|deviceCount|Int64|Contagem resumida de dispositivos da análise da experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|cpuSpikeTimePercentage|Duplo|Tempo de pico da CPU em porcentagem. Valores válidos de 0 a 100|
|ramSpikeTimePercentage|Duplo|Tempo de pico de RAM em porcentagem. Valores válidos de 0 a 100|
|cpuSpikeTimeScore|Int32|A pontuação de tempo de pico da CPU do dispositivo de análise de experiência do usuário. Valores válidos de 0 a 100|
|cpuSpikeTimePercentageThreshold|Duplo|Limite de cpuSpikeTimeScore. Valores válidos de 0 a 100|
|ramSpikeTimeScore|Int32|A pontuação do tempo de pico de RAM do dispositivo de análise de experiência do usuário. Valores válidos de 0 a 100|
|ramSpikeTimePercentageThreshold|Duplo|Limite de ramSpikeTimeScore. Valores válidos de 0 a 100|
|deviceResourcePerformanceScore|Int32|Pontuação de desempenho de recursos de um dispositivo específico. Valores válidos de 0 a 100|
|averageSpikeTimeScore|Int32|AverageSpikeTimeScore de um dispositivo ou um tipo de modelo. Valores válidos de 0 a 100|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsResourcePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "deviceCount": 1024,
  "manufacturer": "String",
  "cpuSpikeTimePercentage": "4.2",
  "ramSpikeTimePercentage": "4.2",
  "cpuSpikeTimeScore": 1024,
  "cpuSpikeTimePercentageThreshold": "4.2",
  "ramSpikeTimeScore": 1024,
  "ramSpikeTimePercentageThreshold": "4.2",
  "deviceResourcePerformanceScore": 1024,
  "averageSpikeTimeScore": 1024
}
```



