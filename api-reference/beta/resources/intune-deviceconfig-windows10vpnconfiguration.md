---
title: tipo de recurso de windows10VpnConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.
author: tfitzmac
ms.openlocfilehash: 1dbbdb5a7065214ab6a290215f2c6016f8ad74bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340695"
---
# <a name="windows10vpnconfiguration-resource-type"></a>tipo de recurso de windows10VpnConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.

Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Obter windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Criar windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Crie um novo objeto de [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|
|[Excluir windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|Nenhum|Exclui um [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).|
|[Atualizar windows10VpnConfiguration](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|Atualize as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .|

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
|connectionName|String|Nome da Conexão exibida para o usuário. Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|servidores|coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Lista de servidores VPN na rede. Verifique se os usuários finais podem acessar esses locais de rede. Esta coleção pode conter um máximo de 500 elementos. Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Binária|Comandos XML personalizados que configura a conexão VPN. (Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|profileTarget|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|Tipo de perfil de destino. Os valores possíveis são: `user`, `device`, `autoPilotDevice`.|
|connectionType|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|Tipo de Conexão. Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.|
|enableSplitTunneling|Boolean|Habilite o túnel em divisão.|
|enableAlwaysOn|Boolean|Habilite o modo Always On.|
|enableDeviceTunnel|Boolean|Habilite o túnel de dispositivo.|
|enableDnsRegistration|Boolean|Habilite o registro de endereço IP com DNS interno.|
|dnsSuffixes|String collection|Especifica os sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.|
|authenticationMethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|Método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.|
|rememberUserCredentials|Boolean|Lembre-se as credenciais do usuário.|
|enableConditionalAccess|Boolean|Habilite o acesso condicional.|
|enableSingleSignOnWithAlternateCertificate|Boolean|Habilite logon único (SSO) com o certificado alternativo.|
|singleSignOnEku|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)|Single sign-on chave EKU (uso estendido).|
|singleSignOnIssuerHash|String|Hash de emissor de logon único.|
|eapXml|Binária|Protocolo de autenticação extensível (EAP) XML. (Matriz de bytes codificados em UTF8)|
|proxyServer|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|Servidor proxy.|
|associatedApps|coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)|Aplicativos associados. Essa coleção pode conter um máximo de 10.000 elementos.|
|onlyAssociatedAppsCanUseConnection|Boolean|Apenas os aplicativos associados podem usar a conexão (-app VPN).|
|windowsInformationProtectionDomain|String|Domínio de proteção de informações do Windows (WIP) para associar a essa conexão.|
|trafficRules|coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)|Regras de tráfego. Essa coleção pode conter um máximo de 1.000 elementos.|
|rotas|coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)|Roteia (opcional para provedores de terceiros). Essa coleção pode conter um máximo de 1.000 elementos.|
|dnsRules|coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)|Regras DNS. Essa coleção pode conter um máximo de 1000 elementos.|

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
|identityCertificate|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Certificado de identidade para autenticação de cliente quando o método de autenticação é o certificado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String"
    }
  ]
}
```





