---
title: tipo de recurso userExperienceAnalyticsAppHealthOSVersionPerformance
description: A entidade de desempenho do dispositivo de análise de so da experiência do usuário contém detalhes de desempenho da versão do sistema operacional.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6d3abfa1330514b48d2df2d5f61ef78e3a85bac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081960"
---
# <a name="userexperienceanalyticsapphealthosversionperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthOSVersionPerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise de so da experiência do usuário contém detalhes de desempenho da versão do sistema operacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthOSVersionPerformances](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-list.md)|coleção [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .|
|[Obter userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-get.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .|
|[Criar userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-create.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .|
|[Excluir userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).|
|[Atualizar userExperienceAnalyticsAppHealthOSVersionPerformance](../api/intune-devices-userexperienceanalyticsapphealthosversionperformance-update.md)|[userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho da versão da experiência do usuário do Analytics OS.|
|osVersion|String|A versão do sistema operacional instalada no dispositivo.|
|osBuildNumber|Cadeia de caracteres|O número de compilação do sistema operacional instalado no dispositivo.|
|activeDeviceCount|Int32|O número de dispositivos ativos para a versão do sistema operacional. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailureInMinutes|Int32|O tempo médio de falha para a versão do sistema operacional em minutos. Valores válidos-2147483648 a 2147483647|
|osVersionAppHealthScore|Duplo|A pontuação de integridade do aplicativo da versão do sistema operacional. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|osVersionAppHealthStatus|Cadeia de caracteres|O status de integridade geral do aplicativo da versão do sistema operacional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "String (identifier)",
  "osVersion": "String",
  "osBuildNumber": "String",
  "activeDeviceCount": 1024,
  "meanTimeToFailureInMinutes": 1024,
  "osVersionAppHealthScore": "4.2",
  "osVersionAppHealthStatus": "String"
}
```






