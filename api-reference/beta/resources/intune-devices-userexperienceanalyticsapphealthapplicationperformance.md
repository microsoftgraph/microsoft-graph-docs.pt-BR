---
title: tipo de recurso userExperienceAnalyticsAppHealthApplicationPerformance
description: A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5c6e2c9292d11cc1a7384d0213a0adbd85921c3
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793170"
---
# <a name="userexperienceanalyticsapphealthapplicationperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthApplicationPerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do aplicativo de análise da experiência do usuário contém detalhes de desempenho do aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthApplicationPerformances](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-list.md)|coleção [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Obter userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-get.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Criar userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-create.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|
|[Excluir userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthApplicationPerformance](../api/intune-devices-userexperienceanalyticsapphealthapplicationperformance-update.md)|[userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appFriendlyName|String|O nome amigável do aplicativo.|
|appPublisher|String|O fornecedor do aplicativo.|
|activeDevices|Int32|O número de dispositivos em que o aplicativo está ativo. Valores válidos-2147483648 a 2147483647|
|totalAppUsageDuration|Int32|O tempo total de uso do aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|totalAppCrashes|Int32|O número de falhas para o aplicativo. Valores válidos-2147483648 a 2147483647|
|totalAppHangs|Int32|O número de suspensões para o aplicativo. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailure|Int32|O tempo médio de falha para o aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|appHealthScore|Duplo|A pontuação de integridade do aplicativo. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|appHealthStatus|String|O status de integridade geral do aplicativo.|
|allOrgsHealthScore|Duplo|A pontuação de integridade mediana do aplicativo em todas as organizações. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|allOrgsMeanTimeToFailure|Int32|O tempo médio de falha em todos os organizações expandidas para o aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|tenantId|String|A ID do locatário associado a este objeto de aplicativo.|
|memaTimeGenerated|String|O momento em que a agregação foi realizada no MEMA.|

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
  "appName": "String",
  "appFriendlyName": "String",
  "appPublisher": "String",
  "activeDevices": 1024,
  "totalAppUsageDuration": 1024,
  "totalAppCrashes": 1024,
  "totalAppHangs": 1024,
  "meanTimeToFailure": 1024,
  "appHealthScore": "4.2",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "4.2",
  "allOrgsMeanTimeToFailure": 1024,
  "tenantId": "String",
  "memaTimeGenerated": "String"
}
```



