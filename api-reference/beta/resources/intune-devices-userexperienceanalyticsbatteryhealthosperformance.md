---
title: tipo de recurso userExperienceAnalyticsBatteryHealthOsPerformance
description: A entidade de desempenho do sistema operacional de análise de experiência do usuário contém informações relacionadas à bateria para todas as versões do sistema operacional em sua organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f0cbc451fb10d12672b60555a08a56803f010a5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697180"
---
# <a name="userexperienceanalyticsbatteryhealthosperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsBatteryHealthOsPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do sistema operacional de análise de experiência do usuário contém informações relacionadas à bateria para todas as versões do sistema operacional em sua organização.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthOsPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-list.md)|[coleção userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Obter userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-get.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Criar userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-create.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|
|[Excluir userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-update.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho da bateria de análise de experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para essa versão do sistema operacional. Valores válidos -2147483648 para 2147483647|
|osVersion|String|Versão do sistema operacional.|
|osBuildNumber|String|Número de com build do sistema operacional.|
|averageMaxCapacityPercentage|Int32|A média da capacidade máxima para todos os dispositivos que executam uma versão específica do sistema operacional. A capacidade máxima mede a capacidade de carga total versus design para as baterias de um dispositivo.. Valores válidos -2147483648 para 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|A média dos tempos de execução estimados em carga total para todos os dispositivos que executam uma versão específica do sistema operacional. Unidade em minutos. Valores válidos -2147483648 para 2147483647|
|averageBatteryAgeInDays|Int32|A média da idade da bateria para todos os dispositivos que executam uma determinada versão do sistema operacional em um locatário. Unidade em dias. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "osVersion": "String",
  "osBuildNumber": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024
}
```



