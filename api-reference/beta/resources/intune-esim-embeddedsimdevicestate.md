---
title: tipo de recurso de embeddedSIMDeviceState
description: Descreve o incorporado SIM código implantação estado de ativação em relação um dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a79453c8d8bcb5682da64ce480f1a2f9f210a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415569"
---
# <a name="embeddedsimdevicestate-resource-type"></a>tipo de recurso de embeddedSIMDeviceState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Descreve o incorporado SIM código implantação estado de ativação em relação um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|coleção [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Lista as propriedades e os relacionamentos dos objetos [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Obter embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Leia as propriedades e os relacionamentos do objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Criar embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Crie um novo objeto de [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Excluir embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|Nenhum|Exclui um [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[Atualizar embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Atualize as propriedades de um objeto [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o status do dispositivo SIM incorporado. Valor atribuído quando criado gerado pelo sistema.|
|createdDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi criado. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que o status do dispositivo SIM incorporado foi modificado pela última vez. Lado de serviços atualizado.|
|lastSyncDateTime|DateTimeOffset|A hora em que o dispositivo SIM incorporado último check-in. Lado de serviços atualizado.|
|universalIntegratedCircuitCardIdentifier|String|O Universal circuito integrado cartão identificador (UICCID) que identifica o hardware no qual um perfil é a serem implantados.|
|deviceName|String|Nome do dispositivo para o qual a assinatura foi provisionado por exemplo, JOE de área de trabalho|
|userName|Cadeia de caracteres|Nome de usuário que a assinatura foi provisionada para ex.: joe@contoso.com|
|estado|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|O estado da operação perfil aplicado ao dispositivo. Os valores possíveis são: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|Descrição do estado do provisionamento de cadeia de caracteres.|

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




