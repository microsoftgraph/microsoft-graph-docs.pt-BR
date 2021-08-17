---
title: Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: A entidade de desempenho do aplicativo de análise de experiência do usuário contém detalhes de desempenho do aplicativo pela versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04c2d807a24b09b91778a6696c1aba75e5dc0bc2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263937"
---
# <a name="userexperienceanalyticsapphealthappperformancebyosversion-resource-type"></a>Tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByOSVersion

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise de experiência do usuário contém detalhes de desempenho do aplicativo pela versão do sistema operacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthAppPerformanceByOSVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-list.md)|[coleção userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Obter userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|
|[Excluir userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).|
|[Atualizar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho de versão do aplicativo de análise de experiência do usuário.|
|osVersion|String|A versão do sistema operacional do aplicativo.|
|osBuildNumber|Cadeia de caracteres|O número de com build do sistema operacional do aplicativo.|
|activeDeviceCount|Int32|O número de dispositivos em que o aplicativo está ativo. Valores válidos -2147483648 para 2147483647|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo.|
|appPublisher|Cadeia de caracteres|O editor do aplicativo.|
|appUsageDuration|Int32|O tempo total de uso do aplicativo em minutos. Valores válidos -2147483648 para 2147483647|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos -2147483648 para 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo de falha média do aplicativo em minutos. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```




