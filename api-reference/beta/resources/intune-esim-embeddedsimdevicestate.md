---
title: Tipo de recurso embeddedSIMDeviceState
description: Descreve o estado de implantação do código de ativação do SIM incorporado em relação a um dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f5b98cbf3d70514b09a18ccd6d9eab7033c862c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039858"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Tipo de recurso embeddedSIMDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o estado de implantação do código de ativação do SIM incorporado em relação a um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[Coleção embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Listar propriedades e relações dos [objetos EMBEDDEDSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Obter embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Leia propriedades e relações do [objeto embeddedSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Criar embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Crie um novo [objeto EMBEDDEDSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Excluir embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|Nenhum|Exclui [umSIMDeviceState incorporado.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Atualizar embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Atualize as propriedades de [um objeto EMBEDDEDSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o status do dispositivo SIM incorporado. Valor gerado pelo sistema atribuído quando criado.|
|createdDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi criado. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez. Lado do serviço atualizado.|
|lastSyncDateTime|DateTimeOffset|A última vez que o dispositivo SIM incorporado se registrou. Lado do serviço atualizado.|
|universalIntegratedCircuitCardIdentifier|Cadeia de Caracteres|O Identificador de Placa de Circuito Integrado Universal (UICCID) identificando o hardware no qual um perfil deve ser implantado.|
|deviceName|String|Nome do dispositivo para o qual a assinatura foi provisionada, por exemplo, DESKTOP-JOE|
|userName|Cadeia de caracteres|Nome de usuário para o qual a assinatura foi provisionada, por exemplo, joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|O estado da operação de perfil aplicada ao dispositivo. Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|Cadeia de Caracteres|Descrição da cadeia de caracteres do estado de provisionamento.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```



