---
title: Tipo de recurso userExperienceAnalyticsBatteryHealthModelPerformance
description: A entidade de desempenho do modelo de avaliação de bateria da experiência do usuário contém informações relacionadas à bateria para todos os modelos de dispositivo exclusivos em sua organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae520e7123f14b48edbbb771d34a3bec0c9b76cd
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687828"
---
# <a name="userexperienceanalyticsbatteryhealthmodelperformance-resource-type"></a>Tipo de recurso userExperienceAnalyticsBatteryHealthModelPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do modelo de avaliação de bateria da experiência do usuário contém informações relacionadas à bateria para todos os modelos de dispositivo exclusivos em sua organização.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthModelPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-list.md)|[coleção userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Obter userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-get.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Criar userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-create.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|
|[Excluir userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthModelPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance-update.md)|[userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do modelo de desempenho da bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para esse modelo. Valores válidos -2147483648 para 2147483647|
|modelo|String|O nome do modelo do dispositivo.|
|fabricante|String|Nome do fabricante do dispositivo.|
|averageMaxCapacityPercentage|Int32|A média da capacidade máxima para todos os dispositivos de um determinado modelo. A capacidade máxima mede a capacidade de carga total versus design para as baterias de um dispositivo.. Valores válidos -2147483648 para 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|A média dos tempos de execução estimados em carga total para todos os dispositivos de um determinado modelo. Unidade em minutos. Valores válidos -2147483648 para 2147483647|
|averageBatteryAgeInDays|Int32|A média da idade da bateria para todos os dispositivos de um determinado modelo em um locatário. Unidade em dias. Valores válidos -2147483648 para 2147483647|

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
  "averageBatteryAgeInDays": 1024
}
```



