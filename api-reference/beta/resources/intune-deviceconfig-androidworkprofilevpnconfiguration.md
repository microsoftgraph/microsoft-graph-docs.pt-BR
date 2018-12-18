---
title: tipo de recurso de androidWorkProfileVpnConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Android perfil de trabalho para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.
author: tfitzmac
ms.openlocfilehash: 6ecda0545e4b8dac23fd0acd6188c14e03fb4185
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324512"
---
# <a name="androidworkprofilevpnconfiguration-resource-type"></a>tipo de recurso de androidWorkProfileVpnConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Android perfil de trabalho para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidWorkProfileVpnConfigurations](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-list.md)|coleção [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .|
|[Obter androidWorkProfileVpnConfiguration](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-get.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .|
|[Criar androidWorkProfileVpnConfiguration](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-create.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Crie um novo objeto de [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .|
|[Excluir androidWorkProfileVpnConfiguration](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-delete.md)|Nenhum|Exclui um [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).|
|[Atualizar androidWorkProfileVpnConfiguration](../api/intune-deviceconfig-androidworkprofilevpnconfiguration-update.md)|[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)|Atualize as propriedades de um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .|

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
|connectionName|String|Nome da Conexão exibida para o usuário.|
|connectionType|[androidWorkProfileVpnConnectionType](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|Tipo de Conexão. Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.|
|role|String|Função quando o tipo de conexão está definida como pulso seguro.|
|território|String|Território quando o tipo de conexão está definida como pulso seguro.|
|servidores|coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Lista de servidores VPN na rede. Verifique se os usuários finais podem acessar esses locais de rede. Esta coleção pode conter um máximo de 500 elementos.|
|impressão digital|String|Impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, que só é aplicável quando o tipo de conexão é verificar Point Cápsula VPN.|
|customData|coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Dados personalizados quando o tipo de conexão está definida como Citrix. Essa coleção pode conter um máximo de 25 elementos.|
|customKeyValueData|Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Dados personalizados quando o tipo de conexão está definida como Citrix. Essa coleção pode conter um máximo de 25 elementos.|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`.|

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
|identityCertificate|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Certificado de identidade para autenticação de cliente quando o método de autenticação é o certificado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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
  "connectionName": "String",
  "connectionType": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "authenticationMethod": "String"
}
```





