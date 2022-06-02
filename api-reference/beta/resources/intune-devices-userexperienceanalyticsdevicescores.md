---
title: Tipo de recurso userExperienceAnalyticsDeviceScores
description: A entidade de pontuações do dispositivo de análise de experiência do usuário consolida as várias pontuações de análise de ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c522277aac0e9122bc597b470102aa2f2aaf4254
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858132"
---
# <a name="userexperienceanalyticsdevicescores-resource-type"></a>Tipo de recurso userExperienceAnalyticsDeviceScores

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de pontuações do dispositivo de análise de experiência do usuário consolida as várias pontuações de análise de ponto de extremidade.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceScoreses](../api/intune-devices-userexperienceanalyticsdevicescores-list.md)|[coleção userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Obter userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-get.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Leia as propriedades e as relações do [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Criar userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-create.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Crie um novo [objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Excluir userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).|
|[Atualizar userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-update.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo de pontuações do dispositivo de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo de análise da experiência do usuário.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|endpointAnalyticsScore|Duplo|A pontuação do dispositivo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|appReliabilityScore|Duplo|A pontuação de confiabilidade do aplicativo de dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|workFromAnywhereScore|Duplo|A pontuação do dispositivo de análise de experiência do usuário funciona em qualquer lugar. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|batteryHealthScore|Duplo|A pontuação de integridade da bateria do dispositivo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade do dispositivo de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2",
  "workFromAnywhereScore": "4.2",
  "batteryHealthScore": "4.2",
  "healthStatus": "String"
}
```




