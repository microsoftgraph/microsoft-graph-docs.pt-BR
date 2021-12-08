---
title: Tipo de recurso hardwareConfigurationDeviceState
description: Contém propriedades para o estado de execução do dispositivo da configuração de hardware
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4700f48823a54bba155841b492e5ff139f05e235
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345348"
---
# <a name="hardwareconfigurationdevicestate-resource-type"></a>Tipo de recurso hardwareConfigurationDeviceState

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de execução do dispositivo da configuração de hardware

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwareConfigurationDeviceStates](../api/intune-deviceconfig-hardwareconfigurationdevicestate-list.md)|[Coleção hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Listar propriedades e relações dos [objetos hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Obter hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-get.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Ler propriedades e relações do [objeto hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Criar hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-create.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Crie um novo [objeto hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|
|[Excluir hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-delete.md)|Nenhum|Exclui um [hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md).|
|[Atualizar hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-update.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Atualize as propriedades de [um objeto hardwareConfigurationDeviceState.](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de estado do dispositivo de script de configuração de hardware. Essa propriedade é somente leitura.|
|deviceName|String|O nome do dispositivo|
|osVersion|String|A versão do sistema operacional do dispositivo.|
|upn|Cadeia de caracteres|Nome principal do usuário (UPN).|
|internalVersion|Int32|A versão interna da Política|
|lastStateUpdateDateTime|DateTimeOffset|O último período de data/hora de quando a configuração de hardware foi executada|
|configurationState|[runState](../resources/intune-shared-runstate.md)|Estado de configuração da última execução de configuração de hardware. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|String|Saída da execução da configuração de hardware|
|configurationError|String|Erro da execução da configuração de hardware|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "String (identifier)",
  "deviceName": "String",
  "osVersion": "String",
  "upn": "String",
  "internalVersion": 1024,
  "lastStateUpdateDateTime": "String (timestamp)",
  "configurationState": "String",
  "configurationOutput": "String",
  "configurationError": "String"
}
```




