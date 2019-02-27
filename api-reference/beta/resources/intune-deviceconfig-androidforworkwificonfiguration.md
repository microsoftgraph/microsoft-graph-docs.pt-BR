---
title: tipo de recurso androidForWorkWiFiConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Android para trabalho a se conectar ao ponto de extremidade de Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade Wi-Fi, você pode tornar a conexão Wi-Fi perfeita para o usuário final. Este perfil oferece tipos de segurança limitados e mais simples do que o perfil de Wi-Fi corporativo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4608b295ae35fd1f169a356cd7c652f1a8847995
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175105"
---
# <a name="androidforworkwificonfiguration-resource-type"></a>tipo de recurso androidForWorkWiFiConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Android para trabalho a se conectar ao ponto de extremidade de Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade Wi-Fi, você pode tornar a conexão Wi-Fi perfeita para o usuário final. Este perfil oferece tipos de segurança limitados e mais simples do que o perfil de Wi-Fi corporativo.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidForWorkWiFiConfigurations](../api/intune-deviceconfig-androidforworkwificonfiguration-list.md)|coleção [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|Listar Propriedades e relações dos objetos [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .|
|[Obter androidForWorkWiFiConfiguration](../api/intune-deviceconfig-androidforworkwificonfiguration-get.md)|[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|Leia as propriedades e as relações do objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .|
|[Criar androidForWorkWiFiConfiguration](../api/intune-deviceconfig-androidforworkwificonfiguration-create.md)|[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|Criar um novo objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .|
|[Excluir androidForWorkWiFiConfiguration](../api/intune-deviceconfig-androidforworkwificonfiguration-delete.md)|Nenhum|Exclui [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).|
|[Atualizar androidForWorkWiFiConfiguration](../api/intune-deviceconfig-androidforworkwificonfiguration-update.md)|[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|Atualiza as propriedades de um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|NetworkName|String|Nome da rede|
|SSID|String|Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.|
|connectAutomatically|Booliano|Conectar automaticamente quando esta rede estiver no intervalo. A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.|
|connectWhenNetworkNameIsHidden|Booliano|Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.|
|à|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP. Os valores possíveis são: `open`, `wpaEnterprise`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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
  "@odata.type": "microsoft.graph.androidForWorkWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String"
}
```




