---
title: Tipo de recurso userExperienceAnalyticsModelScores
description: A entidade de pontuações do modelo de análise de experiência do usuário consolida as várias pontuações de análise de ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbf00cd94e9667ac556535b5d8dca75e2a76800a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857866"
---
# <a name="userexperienceanalyticsmodelscores-resource-type"></a>Tipo de recurso userExperienceAnalyticsModelScores

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de pontuações do modelo de análise de experiência do usuário consolida as várias pontuações de análise de ponto de extremidade.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsModelScoreses](../api/intune-devices-userexperienceanalyticsmodelscores-list.md)|[coleção userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Obter userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-get.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Leia as propriedades e as relações do [objeto userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Criar userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-create.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Crie um novo [objeto userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Excluir userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).|
|[Atualizar userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-update.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de pontuações do modelo de análise de experiência do usuário.|
|modelo|String|Um identificador exclusivo das pontuações do modelo de análise de experiência do usuário: modelo de dispositivo.|
|fabricante|String|Um identificador exclusivo das pontuações do modelo de análise de experiência do usuário: fabricante do dispositivo.|
|modelDeviceCount|Int64|A contagem de dispositivos do modelo de análise de experiência do usuário. Valores válidos -9.22337203685478E+18 a 9.22337203685478E+18|
|endpointAnalyticsScore|Duplo|A pontuação do modelo de análise da experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|appReliabilityScore|Duplo|A pontuação de confiabilidade do aplicativo de modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|workFromAnywhereScore|Duplo|A pontuação do modelo de análise de experiência do usuário funciona em qualquer lugar. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|batteryHealthScore|Duplo|A pontuação de integridade da bateria do modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade do modelo de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsModelScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2",
  "workFromAnywhereScore": "4.2",
  "batteryHealthScore": "4.2",
  "healthStatus": "String"
}
```




