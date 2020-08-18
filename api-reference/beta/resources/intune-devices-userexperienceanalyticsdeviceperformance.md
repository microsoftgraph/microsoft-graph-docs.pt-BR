---
title: tipo de recurso userExperienceAnalyticsDevicePerformance
description: A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho de inicialização do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c4325ac78a1fc5f91c92fc4633d9d10146afd86
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790389"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho de inicialização do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDevicePerformances](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Obter userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Criar userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Criar um novo objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Excluir userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|Nenhum|Exclui [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).|
|[Atualizar userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[função summarizeDevicePerformanceDevices](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo de análise da experiência do usuário.|
|modelo|String|O modelo de dispositivo de análise da experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise da experiência do usuário.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|O tipo de disco do dispositivo de análise da experiência do usuário. Os valores possíveis são: `unkown`, `hdd`, `ssd`.|
|operatingSystemVersion|String|A versão do sistema operacional do dispositivo de análise da experiência do usuário.|
|bootScore|Int32|A pontuação de inicialização do dispositivo de análise da experiência do usuário.|
|coreBootTimeInMs|Int32|O tempo de inicialização do núcleo do dispositivo de análise da experiência do usuário em milissegundos.|
|groupPolicyBootTimeInMs|Int32|O tempo de inicialização da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de integridade do dispositivo de análise da experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32|O placar de logon do dispositivo de análise da experiência do usuário.|
|coreLoginTimeInMs|Int32|O tempo de logon do dispositivo de análise da experiência do usuário em milissegundos.|
|groupPolicyLoginTimeInMs|Int32|O tempo de logon da política de grupo do dispositivo de análise da experiência do usuário em milissegundos.|
|deviceCount|Int64|Contagem de dispositivos resumida da análise de experiência do usuário.|
|responsiveDesktopTimeInMs|Int32|O tempo de resposta da análise da experiência do usuário em milissegundos.|
|blueScreenCount|Int32|Número de telas azuis nos últimos 14 dias. Valores válidos de 0 a 9999999|
|restartCount|Int32|Número de reinicializações nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageBlueScreens|Duplo|Média (média) número de telas azuis por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageRestarts|Duplo|Média (média) número de reinicializações por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "diskType": "String",
  "operatingSystemVersion": "String",
  "bootScore": 1024,
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "healthStatus": "String",
  "loginScore": 1024,
  "coreLoginTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "deviceCount": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "blueScreenCount": 1024,
  "restartCount": 1024,
  "averageBlueScreens": "4.2",
  "averageRestarts": "4.2"
}
```



