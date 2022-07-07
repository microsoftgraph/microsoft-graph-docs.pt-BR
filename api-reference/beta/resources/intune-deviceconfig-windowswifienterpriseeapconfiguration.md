---
title: Tipo de recurso windowsWifiEnterpriseEAPConfiguration
description: Essa entidade fornece descrições dos métodos, propriedades e relações declarados expostos pelo CSP wifi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d9ae39941d82aa7424b702944f40ca2a3c1b14d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668738"
---
# <a name="windowswifienterpriseeapconfiguration-resource-type"></a>Tipo de recurso windowsWifiEnterpriseEAPConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade fornece descrições dos métodos, propriedades e relações declarados expostos pelo CSP wifi.


Herda de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsWifiEnterpriseEAPConfigurations](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-list.md)|[coleção windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Listar propriedades e relações dos [objetos windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Obter windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-get.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Ler propriedades e relações do objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Criar windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-create.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Crie um novo [objeto windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Excluir windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-delete.md)|Nenhum|Exclui um [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).|
|[Atualizar windowsWifiEnterpriseEAPConfiguration](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-update.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Atualize as propriedades de um [objeto windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|preSharedKey|Cadeia de caracteres|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Especifique o tipo de segurança Wifi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Especifique o tipo de limite de conexão limitada para a conexão wi-fi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os valores possíveis são: `unrestricted`, `fixed`, `variable`.|
|Ssid|String|Especifique o SSID da conexão wi-fi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkName|Cadeia de caracteres|Especifique o nome da configuração de rede. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectAutomatically|Boolean|Especifique se a conexão wi-fi deve se conectar automaticamente quando estiver no intervalo. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolean|Especifique se a conexão wi-fi deve se conectar a mais redes preferenciais quando já estiver conectada a essa.  Requer que o ConnectAutomatically seja verdadeiro. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Especifique se a conexão wi-fi deve se conectar automaticamente mesmo quando o SSID não estiver transmitindo. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Especifique a configuração de proxy Wi-Fi configuração Herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|Cadeia de caracteres|Especifique o endereço IP do servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyManualPort|Int32|Especifique a porta para o servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|Cadeia de caracteres|Especifique a URL para o script de configuração do servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|forceFIPSCompliance|Boolean|Especifique se a conformidade com o FIPS deve ser forçada. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|Especifique o tipo de logon único de rede. Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.|
|maximumAuthenticationTimeoutInSeconds|Int32|Especifique o tempo limite máximo de autenticação (em segundos).  Intervalo válido: 1 a 120|
|userBasedVirtualLan|Boolean|Especifica se a LAN virtual usada pelo dispositivo deve ser alterada com base nas credenciais do usuário. Não pode ser usado quando NetworkSingleSignOnType está definido como Desabilitado.|
|promptForAdditionalAuthenticationCredentials|Boolean|Especifique se a conexão wi-fi deve solicitar credenciais de autenticação adicionais.|
|enablePairwiseMasterKeyCaching|Boolean|Especifique se a conexão wi-fi deve habilitar o cache de chaves mestras emparelhadas.|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|Especifique o tempo máximo de cache de chave mestra par (em minutos).  Intervalo válido: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|Especifique o número máximo de chaves mestras emparelhadas no cache.  Intervalo válido: 1 a 255|
|enablePreAuthentication|Boolean|Especifique se a pré-autenticação deve ser habilitada.|
|maximumPreAuthenticationAttempts|Int32|Especifique o máximo de tentativas de pré-autenticação.  Intervalo válido: 1 a 16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de autenticação extensível (EAP). Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Coleção de cadeias de caracteres|Especifique nomes de certificado de servidor confiável.|
|Authenticationmethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Especifique o método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Especifique o protocolo de autenticação interna para EAP TTLS. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Cadeia de caracteres|Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar OAP TTLS ou PEAP.|
|requireCryptographicBinding|Boolean|Especifique se a associação criptográfica deve ser habilitada quando o tipo EAP for selecionado como PEAP.|
|performServerValidation|Boolean|Especifique se a verificação da identidade do servidor deve ser habilitada validando o certificado quando o tipo de EAP for selecionado como PEAP.|
|disableUserPromptForServerValidation|Boolean|Especifique se deve impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo de EAP for selecionado como PEAP.|
|authenticationPeriodInSeconds|Int32|Especifique o número de segundos para o cliente aguardar após uma tentativa de autenticação antes de falhar. Intervalo válido de 1 a 3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação. Intervalo válido de 1 a 3600.|
|eapolStartPeriodInSeconds|Int32|Especifique o número de segundos de espera antes de enviar uma mensagem inicial do EAPOL (Protocolo de Autenticação Extensível via LAN). Intervalo válido de 1 a 3600.|
|maximumEAPOLStartMessages|Int32|Especifique o número máximo de mensagens de início EAPOL (Protocolo de Autenticação Extensível por LAN) a serem enviadas antes de retornar a falha. Intervalo válido de 1 a 100.|
|maximumAuthenticationFailures|Int32|Especifique o máximo de falhas de autenticação permitidas para um conjunto de credenciais. Intervalo válido de 1 a 100.|
|cacheCredentials|Boolean|Especifique se as credenciais do usuário devem ser armazenadas em cache no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem.|
|Authenticationtype|[wifiAuthenticationType](../resources/intune-deviceconfig-wifiauthenticationtype.md)|Especifique se deseja autenticar o usuário, o dispositivo ou usar a autenticação de convidado (nenhuma). Se você estiver usando a autenticação de certificado, verifique se o tipo de certificado corresponde ao tipo de autenticação. Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.|

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
|rootCertificatesForServerValidation|[coleção windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Especifique o certificado raiz para validação do servidor. Esta coleção pode conter um máximo de 500 elementos.|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Especifique o certificado de identidade para autenticação do cliente.|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Especifique o certificado raiz para validação do cliente.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 1024,
  "authenticationRetryDelayPeriodInSeconds": 1024,
  "eapolStartPeriodInSeconds": 1024,
  "maximumEAPOLStartMessages": 1024,
  "maximumAuthenticationFailures": 1024,
  "cacheCredentials": true,
  "authenticationType": "String"
}
```




