---
title: tipo de recurso userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory
description: A entidade histórico de tempo de execução da bateria de análise de experiência do usuário contém a tendência de tempo de execução de um dispositivo em um período de 30 dias
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db4d43edf29e295a2fcae26b03f2dcfad83fde70
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695501"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceruntimehistory-resource-type"></a>tipo de recurso userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade histórico de tempo de execução da bateria de análise de experiência do usuário contém a tendência de tempo de execução de um dispositivo em um período de 30 dias

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsBatteryHealthDeviceRuntimeHistories](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-list.md)|[coleção userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Obter userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-get.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Criar userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-create.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Crie um novo [objeto userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|
|[Excluir userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md).|
|[Atualizar userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory-update.md)|[userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceruntimehistory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de tempo de execução da bateria de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo, id do dispositivo Intune DeviceID ou SCCM.|
|runtimeDateTime|String|O tempo de data para a instância do histórico de tempo de execução.|
|estimatedRuntimeInMinutes|Int32|O tempo de execução estimado do dispositivo quando a bateria é totalmente carregada. Unidade em minutos. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceRuntimeHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "runtimeDateTime": "String",
  "estimatedRuntimeInMinutes": 1024
}
```



