---
title: Tipo de recurso userExperienceAnalyticsBatteryHealthModelPerformance
description: A entidade de desempenho do modelo de integridade da bateria de análise de experiência do usuário contém informações relacionadas à bateria para todos os modelos de dispositivo exclusivos em sua organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 010b4498a8b725519636a727e0fada648c3a2b69
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857425"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>Tipo de recurso userExperienceAnalyticsBatteryHealthModelPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do modelo de integridade da bateria de análise de experiência do usuário contém informações relacionadas à bateria para todos os modelos de dispositivo exclusivos em sua organização.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[coleção userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Obter userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Criar userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|
|[Excluir userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do modelo de integridade da bateria de análise da experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para esse modelo. Valores válidos -2147483648 para 2147483647|
|modelo|String|O nome do modelo do dispositivo.|
|fabricante|String|Nome do fabricante do dispositivo.|
|averageMaxCapacityPercentage|Int32|A média da capacidade máxima para todos os dispositivos de um determinado modelo. A capacidade máxima mede a carga total versus a capacidade de design das baterias de um dispositivo.. Valores válidos -2147483648 para 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|A média dos runtimes estimados com custo total para todos os dispositivos de um determinado modelo. Unidade em minutos. Valores válidos -2147483648 para 2147483647|
|averageBatteryAgeInDays|Int32|A média da duração da bateria para todos os dispositivos de um determinado modelo em um locatário. Unidade em dias. Valores válidos -2147483648 para 2147483647|
|modelBatteryHealthScore|Int32|Uma média ponderada da pontuação máxima de capacidade de um modelo e da pontuação de estimativa de runtime. Os valores variam de 0 a 100. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "model": "String",
  "manufacturer": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024,
  "modelBatteryHealthScore": 1024
}
```




