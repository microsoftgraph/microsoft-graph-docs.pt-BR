---
title: tipo de recurso userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8857c6a392437335c7324c139fa0b2c9880b12a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733969"
---
# <a name="userexperienceanalyticsapphealthdeviceperformancedetails-resource-type"></a>tipo de recurso userExperienceAnalyticsAppHealthDevicePerformanceDetails

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsAppHealthDevicePerformanceDetailses](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-list.md)|coleção [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Obter userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-get.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-create.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Criar um novo objeto [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|
|[Excluir userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-delete.md)|Nenhum|Exclui [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).|
|[Atualizar userExperienceAnalyticsAppHealthDevicePerformanceDetails](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails-update.md)|[userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|eventType|String|O tipo do evento.|
|appDisplayName|String|O nome amigável do aplicativo para o qual o evento ocorreu.|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
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
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```





