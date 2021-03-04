---
title: tipo de recurso userExperienceAnalyticsAppHealthApplicationPerformance
description: A entidade de desempenho do aplicativo de análise de experiência do usuário contém detalhes de desempenho do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c463184c0039885401720cb123fc33c9e51ce77
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433093"
---
# <a name="userexperienceanalyticsapphealthapplicationperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthApplicationPerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise de experiência do usuário contém detalhes de desempenho do aplicativo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthApplicationPerformances](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-list.md)|[coleção userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|
|[Obter userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-get.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|
|[Criar userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-create.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|
|[Excluir userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-update.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthApplicationPerformance.](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do aplicativo de análise de experiência do usuário.|
|appHangCount|Int32|O número de travas para o aplicativo. Valores válidos -2147483648 a 2147483647|
|appHealthScore|Duplo|A pontuação de saúde do aplicativo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|appHealthStatus|String|O status de saúde geral do aplicativo.|
|allOrgsHealthScore|Duplo|A pontuação de saúde mediana do aplicativo em todas as organizações. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308.|
|activeDeviceCount|Int32|O número de dispositivos em que o aplicativo está ativo. Valores válidos -2147483648 a 2147483647|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|String|O nome amigável do aplicativo.|
|appPublisher|String|O editor do aplicativo.|
|appUsageDuration|Int32|O tempo total de uso do aplicativo em minutos. Valores válidos -2147483648 a 2147483647|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos -2147483648 a 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo de falha média do aplicativo em minutos. Valores válidos -2147483648 a 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "String (identifier)",
  "appHangCount": 1024,
  "appHealthScore": "4.2",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "4.2",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```




