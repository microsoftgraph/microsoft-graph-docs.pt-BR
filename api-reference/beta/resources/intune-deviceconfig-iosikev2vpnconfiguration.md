---
title: Tipo de recurso iosikEv2VpnConfiguration
description: Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo iOS a se conectar ao ponto de extremidade vpn IKEv2 desejado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c89f0f2a8dc6d31c659e131da5101852abfd77f7
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671343"
---
# <a name="iosikev2vpnconfiguration-resource-type"></a>Tipo de recurso iosikEv2VpnConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo iOS a se conectar ao ponto de extremidade vpn IKEv2 desejado.


Herda de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosikEv2VpnConfigurations](../api/intune-deviceconfig-iosikev2vpnconfiguration-list.md)|[Coleção iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Listar propriedades e relações dos objetos [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .|
|[Obter iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-get.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Ler propriedades e relações do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .|
|[Criar iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-create.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Crie um novo [objeto iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .|
|[Excluir iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-delete.md)|Nenhum|Exclui um [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).|
|[Atualizar iosikEv2VpnConfiguration](../api/intune-deviceconfig-iosikev2vpnconfiguration-update.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|Atualize as propriedades de um [objeto iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Connectionname|Cadeia de Caracteres|Nome da conexão exibido para o usuário. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Connectiontype|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Tipo de conexão. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Os valores possíveis são: , , , , , , , , `citrix``ciscoIPSec`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, , `ikEv2`, , `alwaysOn`, . `microsoftTunnel``microsoftProtect``netMotionMobility``customVpn``checkPointCapsuleVpn``dellSonicWallMobileConnect``f5EdgeClient``pulseSecure``ciscoAnyConnect`|
|loginGroupOrDomain|Cadeia de Caracteres|Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|Cadeia de Caracteres|Função quando o tipo de conexão é definido como Pulse Secure. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Reino|Cadeia de Caracteres|Realm quando o tipo de conexão é definido como Pulse Secure. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Servidor VPN na rede. Verifique se os usuários finais podem acessar esse local de rede. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|identificador|Cadeia de Caracteres|Identificador fornecido pelo fornecedor de VPN quando o tipo de conexão é definido como VPN personalizada. Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Customdata|Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)|Dados personalizados quando o tipo de conexão é definido como VPN personalizada. Use este campo para habilitar a funcionalidade não compatível com Intune, mas disponível em sua solução de VPN. Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave-valor. Essa coleção pode conter um máximo de 25 elementos. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|Coleção [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|Dados personalizados quando o tipo de conexão é definido como VPN personalizada. Use este campo para habilitar a funcionalidade não compatível com Intune, mas disponível em sua solução de VPN. Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave-valor. Essa coleção pode conter um máximo de 25 elementos. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|enableSplitTunneling|Booleano|Envie todo o tráfego de rede por meio de VPN. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Authenticationmethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Método de autenticação para essa conexão VPN. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.|
|enablePerApp|Booliano|Definir isso como true cria Per-App conteúdo VPN que pode ser associado posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|safariDomains|Conjunto de cadeias de caracteres|Domínios do Safari quando essa configuração de VPN por aplicativo está habilitada. Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|onDemandRules|[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)|Regras sob demanda. Esta coleção pode conter um máximo de 500 elementos. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Providertype|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|Tipo de provedor para VPN por aplicativo. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.|
|associatedDomains|String collection|Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|excludedDomains|Conjunto de cadeias de caracteres|Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disableOnDemandUserOverride|Booleano|Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdle|Booliano|Se deve se desconectar após ociosidades de conexão sob demanda Herdadas de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|disconnectOnIdleTimerInSeconds|Int32|O período de tempo em segundos a aguardar antes de desconectar uma conexão sob demanda. Valores válidos de 0 a 65535 Herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|Servidor Proxy. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|optInToDeviceIdSharing|Booliano|Opt-In compartilhar a ID do dispositivo com clientes VPN de terceiros para uso durante a validação do controle de acesso à rede. Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|userDomain|Cadeia de Caracteres|Somente Zscaler. Insira um domínio estático com o qual preencher previamente o campo de logon no aplicativo Zscaler. Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|strictEnforcement|Booliano|Somente Zscaler. Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler. "True" significa que o tráfego está bloqueado. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|cloudName|Cadeia de Caracteres|Somente Zscaler. Nuvem Zscaler à qual o usuário está atribuído. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|excludeList|Coleção de cadeias de caracteres|Somente Zscaler. Lista de endereços de rede que não são enviados por meio da nuvem do Zscaler. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|targetedMobileApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Aplicativos móveis direcionados. Esta coleção pode conter um máximo de 500 elementos. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|microsoftTunnelSiteId|Cadeia de Caracteres|ID do site do Microsoft Tunnel. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|childSecurityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Parâmetros de associação de segurança filho|
|clientAuthenticationType|[vpnClientAuthenticationType](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|Tipo de Autenticação de Cliente que o cliente VPN usará. Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.|
|deadPeerDetectionRate|[vpnDeadPeerDetectionRate](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|Determine com que frequência verificar se uma conexão de par ainda está ativa. . Os valores possíveis são: `medium`, `none`, `low`, `high`.|
|disableMobilityAndMultihoming|Boolean|Desabilitar MOBIKE|
|disableRedirect|Booleano|Desabilitar Redirecionamento|
|enableCertificateRevocationCheck|Booleano|Habilita uma verificação de revogação de melhor esforço; tempo limite de resposta do servidor não causará falha|
|enableEAP|Booleano|Habilita a autenticação somente EAP|
|enablePerfectForwardSecrecy|Booleano|Habilitar PFS (Perfect Forward Secrecy).|
|enableUseInternalSubnetAttributes|Booleano|Habilitar usar atributos de sub-rede internas.|
|localIdentifier|[vpnLocalIdentifier](../resources/intune-deviceconfig-vpnlocalidentifier.md)|Método de identificação do cliente que está tentando se conectar via VPN. . Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.|
|remoteIdentifier|Cadeia de Caracteres|Endereço do servidor IKEv2. Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN|
|securityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|Parâmetros de associação de segurança|
|serverCertificateCommonName|Cadeia de Caracteres|Nome comum do Certificado do Servidor IKEv2 usado na Autenticação do Servidor|
|serverCertificateIssuerCommonName|Cadeia de caracteres|Nome comum do emissor do emissor do Certificado do Servidor IKEv2 usado na Autenticação|
|serverCertificateType|[vpnServerCertificateType](../resources/intune-deviceconfig-vpnservercertificatetype.md)|O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação. Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.|
|sharedSecret|Cadeia de Caracteres|Usado quando a Autenticação de Segredo Compartilhado é selecionada|
|tlsMaximumVersion|Cadeia de caracteres|A versão máxima do TLS a ser usada com a autenticação EAP-TLS|
|tlsMinimumVersion|String|A versão mínima do TLS a ser usada com a autenticação EAP-TLS|
|allowDefaultSecurityAssociationParameters|Booliano|Permite o uso de parâmetros de associação de segurança definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.|
|allowDefaultChildSecurityAssociationParameters|Booleano|Permite o uso de parâmetros de associação de segurança filho definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.|
|alwaysOnConfiguration|[appleVpnAlwaysOnConfiguration](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|Configuração AlwaysOn|
|enableAlwaysOnConfiguration|Booleano|Determina se a VPN AlwaysOn está habilitada|
|mtuSizeInBytes|Int32|Unidade de transmissão máxima. Valores válidos de 1280 a 1400|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Certificado de identidade para autenticação de cliente quando o método de autenticação é certificado. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Configurações de nível de locatário para as Credenciais Derivadas a serem usadas para autenticação. Herdado [de iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosikEv2VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "providerType": "String",
  "associatedDomains": [
    "String"
  ],
  "excludedDomains": [
    "String"
  ],
  "disableOnDemandUserOverride": true,
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 1024,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true,
  "userDomain": "String",
  "strictEnforcement": true,
  "cloudName": "String",
  "excludeList": [
    "String"
  ],
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "microsoftTunnelSiteId": "String",
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "clientAuthenticationType": "String",
  "deadPeerDetectionRate": "String",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "String",
  "remoteIdentifier": "String",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "serverCertificateCommonName": "String",
  "serverCertificateIssuerCommonName": "String",
  "serverCertificateType": "String",
  "sharedSecret": "String",
  "tlsMaximumVersion": "String",
  "tlsMinimumVersion": "String",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "String",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "String",
    "airPrintExceptionAction": "String",
    "cellularExceptionAction": "String",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "String"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 1024,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 1024
}
```




