---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Crie um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f44bc822fd9c45d57cd07f0bf1719064dc7dfd58
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790724"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a>Criar windowsWifiEnterpriseEAPConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de Marcas de Escopo para esta instância de Entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|preSharedKey|Cadeia de caracteres|Essa é a chave pré-compartilhada para a rede WPA Personal Wi-Fi rede. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Especifique o Tipo de Segurança Wifi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Especifique o tipo de limite de conexão limitado para a conexão wi-fi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os valores possíveis são: `unrestricted`, `fixed`, `variable`.|
|ssid|Cadeia de caracteres|Especifique o SSID da conexão wi-fi. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkName|Cadeia de caracteres|Especifique o nome da configuração de rede. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectAutomatically|Boolean|Especifique se a conexão wi-fi deve se conectar automaticamente quando estiver dentro do intervalo. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectToPreferredNetwork|Boolean|Especifique se a conexão wi-fi deve se conectar a redes mais preferenciais quando já estiver conectada a esta.  Requer ConnectAutomatically para ser true. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Especifique se a conexão wi-fi deve se conectar automaticamente, mesmo quando o SSID não estiver sendo transmitido. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Especifique a configuração de proxy Wi-Fi Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md). Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|Cadeia de caracteres|Especifique o endereço IP do servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyManualPort|Int32|Especifique a porta para o servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|Cadeia de caracteres|Especifique a URL para o script de configuração do servidor proxy. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|forceFIPSCompliance|Boolean|Especifica se é necessário forçar a conformidade FIPS. Herdado [de windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|Especifique o tipo de sinal único de rede. Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.|
|maximumAuthenticationTimeoutInSeconds|Int32|Especifique o tempo limite máximo de autenticação (em segundos).  Intervalo válido: 1 a 120|
|userBasedVirtualLan|Boolean|Especifica se deve alterar a LAN virtual usada pelo dispositivo com base nas credenciais do usuário. Não pode ser usado quando NetworkSingleSignOnType está definida como Desabilitada.|
|promptForAdditionalAuthenticationCredentials|Boolean|Especifique se a conexão wi-fi deve solicitar credenciais de autenticação adicionais.|
|enablePairwiseMasterKeyCaching|Boolean|Especifique se a conexão wi-fi deve habilitar o cache de chaves mestras pares.|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|Especifique o tempo máximo de cache da chave mestra em pares (em minutos).  Intervalo válido: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|Especifique o número máximo de chaves mestras pares em cache.  Intervalo válido: 1 a 255|
|enablePreAuthentication|Boolean|Especifica se a pré-autenticação deve ser habilitada.|
|maximumPreAuthenticationAttempts|Int32|Especifique o máximo de tentativas de pré-autenticação.  Intervalo válido: 1 a 16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de autenticação extensível (EAP). Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador). Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|trustedServerCertificateNames|Conjunto de cadeias de caracteres|Especifique nomes de certificados de servidor confiáveis.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Especifique o método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Especifique o protocolo de autenticação interna para TTLS EAP. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Cadeia de caracteres|Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar TTLS EAP ou PEAP.|
|requireCryptographicBinding|Boolean|Especifica se a associação criptográfica deve ser habilitada quando o tipo EAP for selecionado como PEAP.|
|performServerValidation|Boolean|Especifique se a verificação da identidade do servidor será habilitada validando o certificado quando o tipo EAP for selecionado como PEAP.|
|disableUserPromptForServerValidation|Boolean|Especifique se deve impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.|
|authenticationPeriodInSeconds|Int32|Especifique o número de segundos para que o cliente aguarde após uma tentativa de autenticação antes de falhar. Intervalo válido de 1 a 3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação. Intervalo válido de 1 a 3600.|
|eapolStartPeriodInSeconds|Int32|Especifique o número de segundos de espera antes de enviar uma mensagem de início EAPOL (Extensible Authentication Protocol over LAN). Intervalo válido de 1 a 3600.|
|maximumEAPOLStartMessages|Int32|Especifica o número máximo de mensagens de início EAPOL (Extensible Authentication Protocol over LAN) a serem enviadas antes da falha de retorno. Intervalo válido de 1 a 100.|
|maximumAuthenticationFailures|Int32|Especifique o máximo de falhas de autenticação permitidas para um conjunto de credenciais. Intervalo válido de 1 a 100.|
|cacheCredentials|Boolean|Especifique se as credenciais do usuário devem ser armazenadas em cache no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem.|
|authenticationType|[wifiAuthenticationType](../resources/intune-deviceconfig-wifiauthenticationtype.md)|Especifique se o usuário, o dispositivo ou a autenticação de convidado devem ser autenticados (nenhum). Se você estiver usando autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação. Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2695

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2867

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




