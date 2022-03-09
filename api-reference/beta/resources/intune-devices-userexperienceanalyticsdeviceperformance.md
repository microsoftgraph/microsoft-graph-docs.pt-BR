---
title: Tipo de recurso userExperienceAnalyticsDevicePerformance
description: A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes do desempenho da inicialização do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 444168c83f34ad8da35f23b0bee27095e495bc4a
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367675"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>Tipo de recurso userExperienceAnalyticsDevicePerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes do desempenho da inicialização do dispositivo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDevicePerformances](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|[coleção userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Obter userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Criar userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Crie um novo [objeto userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Excluir userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|Nenhuma|Exclui um [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).|
|[Atualizar userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[função summarizeDevicePerformanceDevices](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|[coleção userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo de desempenho de inicialização do dispositivo de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo de análise de experiência do usuário.|
|modelo|String|O modelo de dispositivo de análise de experiência do usuário.|
|fabricante|String|O fabricante do dispositivo de análise de experiência do usuário.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|O tipo de disco do dispositivo de análise de experiência do usuário. Os valores possíveis são: `unknown`, `hdd`, `ssd`, `unknownFutureValue`.|
|operatingSystemVersion|String|A versão do sistema operacional do dispositivo de análise de experiência do usuário.|
|bootScore|Int32|A pontuação de inicialização do dispositivo de análise de experiência do usuário.|
|coreBootTimeInMs|Int32|O tempo de inicialização principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyBootTimeInMs|Int32|O tempo de inicialização da política de grupo de dispositivos de análise de experiência do usuário em milissegundos.|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde do dispositivo de análise de experiência do usuário. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32|A pontuação de logon do dispositivo de análise de experiência do usuário.|
|coreLoginTimeInMs|Int32|O tempo de logon principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyLoginTimeInMs|Int32|O tempo de logon da política de grupo de dispositivos de análise de experiência do usuário em milissegundos.|
|deviceCount|Int64|Contagem resumida de dispositivos da análise da experiência do usuário.|
|responsiveDesktopTimeInMs|Int32|A análise da experiência do usuário responde ao tempo da área de trabalho em milissegundos.|
|blueScreenCount|Int32|Número de telas azuis nos últimos 14 dias. Valores válidos de 0 a 9999999|
|restartCount|Int32|Número de reinicializações nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageBlueScreens|Duplo|Número médio (médio) de Telas Azuis por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|
|averageRestarts|Duplo|Número médio (médio) de Reinicializações por dispositivo nos últimos 14 dias. Valores válidos de 0 a 9999999|
|startupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do dispositivo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|modelStartupPerformanceScore|Duplo|A pontuação de desempenho de inicialização do modelo de análise de experiência do usuário. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|

## <a name="relationships"></a>Relações
Nenhuma

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
  "averageRestarts": "4.2",
  "startupPerformanceScore": "4.2",
  "modelStartupPerformanceScore": "4.2"
}
```




