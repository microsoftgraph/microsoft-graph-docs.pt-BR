---
title: tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo por versão do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4c2c0ec5a532be1a9cb3090a4d2a1b6d69cb0fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081964"
---
# <a name="userexperienceanalyticsapphealthappperformancebyappversion-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthAppPerformanceByAppVersion

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo por versão do aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthAppPerformanceByAppVersions](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-list.md)|coleção [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Obter userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-get.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Criar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-create.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|
|[Excluir userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).|
|[Atualizar userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../api/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion-update.md)|[userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.|
|appVersion|Cadeia de caracteres|A versão do aplicativo.|
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
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "String (identifier)",
  "appVersion": "String",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": 1024,
  "appCrashCount": 1024,
  "meanTimeToFailureInMinutes": 1024
}
```






