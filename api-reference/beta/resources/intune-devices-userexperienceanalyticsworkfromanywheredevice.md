---
title: Tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevice
description: O relatório de análise de experiência do usuário Dispositivo para trabalho em qualquer lugar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cef0dd74416c4fbcef83ebe10109795ba41986c1
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665585"
---
# <a name="userexperienceanalyticsworkfromanywheredevice-resource-type"></a>Tipo de recurso userExperienceAnalyticsWorkFromAnywhereDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O relatório de análise de experiência do usuário Dispositivo para trabalho em qualquer lugar

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsWorkFromAnywhereDevices](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-list.md)|[Coleção userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Obter userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-get.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Criar userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-create.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|
|[Excluir userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-delete.md)|Nenhuma|Exclui um [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md).|
|[Atualizar userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-update.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da análise de experiência do usuário funciona em qualquer dispositivo.|
|deviceName|String|O trabalho do nome do dispositivo em qualquer lugar.|
|serialNumber|String|A experiência do usuário funciona de qualquer lugar do número de série do dispositivo.|
|fabricante|String|A experiência do usuário funciona de qualquer fabricante do dispositivo.|
|modelo|String|A experiência do usuário funciona de qualquer lugar do modelo do dispositivo.|
|propriedade|String|A experiência do usuário funciona de qualquer lugar da propriedade do dispositivo.|
|managedBy|String|A experiência do usuário funciona de qualquer lugar do agente de gerenciamento do dispositivo.|
|autoPilotRegistered|Booleano|A experiência do usuário funciona em qualquer lugar do piloto automático do dispositivo intuneRegistered.|
|autoPilotProfileAssigned|Booleano|A análise da experiência do usuário funciona em qualquer lugar do autopilotProfileAssigned do dispositivo intune.|
|azureAdRegistered|Booleano|A experiência do usuário funciona de qualquer lugar do dispositivo azureAdRegistered.|
|azureAdDeviceId|String|A experiência do usuário funciona em qualquer lugar do Azure Ad device Id.|
|azureAdJoinType|String|A experiência do usuário funciona de qualquer lugar do azure Ad joinType do dispositivo.|
|osDescription|Cadeia de caracteres|A experiência do usuário funciona de qualquer lugar da Descrição do sistema operacional do dispositivo.|
|osVersion|String|A experiência do usuário funciona de qualquer lugar da versão do sistema operacional do dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String"
}
```




