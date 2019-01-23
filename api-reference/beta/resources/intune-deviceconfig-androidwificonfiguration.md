---
title: tipo de recurso de androidWiFiConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Android para se conectar ao ponto de extremidade Wi-Fi desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade Wi-Fi que você pode fazer a conexão Wi-Fi perfeita para usuário final. Esse perfil fornece tipos de segurança limitado e mais simples que perfil corporativa Wi-Fi.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 71acee467bdcabd0d82b20d1719cc8a8f73d9c36
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405489"
---
# <a name="androidwificonfiguration-resource-type"></a>tipo de recurso de androidWiFiConfiguration

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Android para se conectar ao ponto de extremidade Wi-Fi desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade Wi-Fi que você pode fazer a conexão Wi-Fi perfeita para usuário final. Esse perfil fornece tipos de segurança limitado e mais simples que perfil corporativa Wi-Fi.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidWiFiConfigurations](../api/intune-deviceconfig-androidwificonfiguration-list.md)|coleção [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .|
|[Obter androidWiFiConfiguration](../api/intune-deviceconfig-androidwificonfiguration-get.md)|[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|Leia as propriedades e os relacionamentos do objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .|
|[Criar androidWiFiConfiguration](../api/intune-deviceconfig-androidwificonfiguration-create.md)|[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|Crie um novo objeto de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .|
|[Excluir androidWiFiConfiguration](../api/intune-deviceconfig-androidwificonfiguration-delete.md)|Nenhum|Exclui um [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).|
|[Atualizar androidWiFiConfiguration](../api/intune-deviceconfig-androidwificonfiguration-update.md)|[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)|Atualize as propriedades de um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|networkName|String|Nome da rede|
|SSID|String|Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.|
|connectAutomatically|Boolean|Conecte automaticamente quando esta rede estiver no intervalo. Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.|
|connectWhenNetworkNameIsHidden|Boolean|Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP. Os valores possíveis são: `open`, `wpaEnterprise`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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




