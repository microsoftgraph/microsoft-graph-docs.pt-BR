---
title: tipo de recurso userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: A entidade de desempenho do dispositivo de análise da experiência do usuário contém detalhes de desempenho do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 834d2e2871e8ddf7366ddc1ea0e77398eeae48f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081959"
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
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do dispositivo de análise da experiência do usuário.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|eventType|Cadeia de caracteres|O tipo do evento.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo para o qual o evento ocorreu.|
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






