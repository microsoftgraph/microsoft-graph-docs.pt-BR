---
title: iosCustomConfiguration resource type
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a91515ddfcbc4932e9615d8253097549f69773b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252837"
---
# <a name="ioscustomconfiguration-resource-type"></a>iosCustomConfiguration resource type

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso iosCustomConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosCustomConfigurations](../api/intune-deviceconfig-ioscustomconfiguration-list.md)|Coleção [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Lista propriedades e relações dos objetos [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|
|[Obter iosCustomConfiguration](../api/intune-deviceconfig-ioscustomconfiguration-get.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Propriedades de leitura e relações do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|
|[Criar iosCustomConfiguration](../api/intune-deviceconfig-ioscustomconfiguration-create.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Cria um novo objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|
|[Excluir iosCustomConfiguration](../api/intune-deviceconfig-ioscustomconfiguration-delete.md)|Nenhum|Exclui um [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|
|[Atualizar iosCustomConfiguration](../api/intune-deviceconfig-ioscustomconfiguration-update.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Atualiza as propriedades de um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|payloadName|String|Nome que é exibido para o usuário.|
|payloadFileName|Cadeia de caracteres|O nome do arquivo de carga (*.mobileconfig | *.xml).|
|payload|Binária|Carga. (Matriz de bytes codificados em UTF8)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```



