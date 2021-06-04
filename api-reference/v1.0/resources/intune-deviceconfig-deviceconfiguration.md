---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82f1de5e835ceba2a15559411a07638dee2602bd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742906"
---
# <a name="deviceconfiguration-resource-type"></a>Tipo de recurso deviceConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração do dispositivo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceConfigurations](../api/intune-deviceconfig-deviceconfiguration-list.md)|Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|[Obter deviceConfiguration](../api/intune-deviceconfig-deviceconfiguration-get.md)|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|[atribuir ação](../api/intune-deviceconfig-deviceconfiguration-assign.md)|Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Ainda não documentado|
|[função getOmaSettingPlainTextValue](../api/intune-deviceconfig-deviceconfiguration-getomasettingplaintextvalue.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|Última modificação de DateTime do objeto.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo.|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo.|
|versão|Int32|Versão da configuração do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo.|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração de dispositivo por dispositivo.|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação de configuração do dispositivo pelo usuário.|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral do status dos dispositivos da configuração de dispositivos|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral do status dos usuários da configuração de dispositivos|
|deviceSettingStateSummaries|Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo do dispositivo do estado de definição de configuração do dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```




