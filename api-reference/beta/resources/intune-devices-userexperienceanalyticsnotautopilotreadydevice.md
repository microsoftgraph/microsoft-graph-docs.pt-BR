---
title: Tipo de recurso userExperienceAnalyticsNotAutopilotReadyDevice
description: Análise da experiência do usuário Dispositivo não windows autopilot pronto.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d09e1c897833839aa2f8581b9ec8ea23e6ad561a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020368"
---
# <a name="userexperienceanalyticsnotautopilotreadydevice-resource-type"></a>Tipo de recurso userExperienceAnalyticsNotAutopilotReadyDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Análise da experiência do usuário Dispositivo não windows autopilot pronto.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsNotAutopilotReadyDevices](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-list.md)|[coleção userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Obter userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-get.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Criar userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-create.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Crie um novo [objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|
|[Excluir userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md).|
|[Atualizar userExperienceAnalyticsNotAutopilotReadyDevice](../api/intune-devices-userexperienceanalyticsnotautopilotreadydevice-update.md)|[userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo intune de análise de experiência do usuário.|
|deviceName|String|O nome do dispositivo intune.|
|serialNumber|String|O número de série do dispositivo intune.|
|fabricante|String|O fabricante do dispositivo intune.|
|modelo|String|O modelo do dispositivo intune.|
|managedBy|Cadeia de caracteres|O dispositivo do intune é gerenciado por.|
|autoPilotRegistered|Boolean|O piloto automático do dispositivo intuneRegistered.|
|autoPilotProfileAssigned|Boleano|O autopilotProfileAssigned do dispositivo intune.|
|azureAdRegistered|Booliano|O dispositivo do intune é azureAdRegistered.|
|azureAdJoinType|Cadeia de Caracteres|O azure Ad joinType do dispositivo do intune.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "String (identifier)",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdJoinType": "String"
}
```



