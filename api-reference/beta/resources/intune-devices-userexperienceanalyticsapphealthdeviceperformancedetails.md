---
title: tipo de recurso userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes de desempenho do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e732dc90d24205ca5d94fad310eca3e5b6f23e31
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256063"
---
# <a name="userexperienceanalyticsapphealthdeviceperformancedetails-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthDevicePerformanceDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise de experiência do usuário contém detalhes de desempenho do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthDevicePerformanceDetailses](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-list.md)|[coleção userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|
|[Obter userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-get.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|
|[Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-create.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Crie um novo [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|
|[Excluir userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).|
|[Atualizar userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-update.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do dispositivo de análise de experiência do usuário.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|eventType|Cadeia de caracteres|O tipo do evento.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo para o qual o evento ocorreu.|
|appPublisher|Cadeia de caracteres|O editor do aplicativo.|
|appVersion|Cadeia de caracteres|A versão do aplicativo.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceDisplayName|Cadeia de caracteres|O nome do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "eventType": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```




