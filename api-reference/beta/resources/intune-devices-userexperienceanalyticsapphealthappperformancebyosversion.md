---
title: tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo por versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 673833ebcdccb90f5d691a7dad9d560da774add3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081963"
---
# <a name="userexperienceanalyticsapphealthappperformancebyosversion-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByOSVersion

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo por versão do sistema operacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthAppPerformanceByOSVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-list.md)|coleção [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Obter userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Criar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|
|[Excluir userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).|
|[Atualizar userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho da versão do aplicativo de análise da experiência do usuário.|
|osVersion|String|A versão do sistema operacional do aplicativo.|
|osBuildNumber|Cadeia de caracteres|O número de compilação do sistema operacional do aplicativo.|
|activeDeviceCount|Int32|O número de dispositivos em que o aplicativo está ativo. Valores válidos-2147483648 a 2147483647|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo.|
|appPublisher|Cadeia de caracteres|O fornecedor do aplicativo.|
|appUsageDuration|Int32|O tempo total de uso do aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|appCrashCount|Int32|O número de falhas para o aplicativo. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo médio de falha para o aplicativo em minutos. Valores válidos-2147483648 a 2147483647|

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






