---
title: Criar windowsWiredNetworkConfiguration
description: Crie um novo objeto windowsWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c56a699ae48c3e0ab77c51e344e095bc9412ef99
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630982"
---
# <a name="create-windowswirednetworkconfiguration"></a>Criar windowsWiredNetworkConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
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
No corpo da solicitação, fornece uma representação JSON para o objeto windowsWiredNetworkConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsWiredNetworkConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|authenticationType|[wiredNetworkAuthenticationType](../resources/intune-deviceconfig-wirednetworkauthenticationtype.md)|Especifique se o usuário, o dispositivo ou o dispositivo devem ser autenticados (nenhum). Se você estiver usando autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação. Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`. Os possíveis valores são: `none`, `user`, `machine`, `machineOrUser`, `guest`, `unknownFutureValue`.|
|cacheCredentials|Boolean|Quando TRUE, armazena em cache as credenciais do usuário no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem. Quando FALSE, não cache credenciais. O valor padrão é FALSE.|
|authenticationPeriodInSeconds|Int32|Especifique o número de segundos para o cliente aguardar após uma tentativa de autenticação antes de falhar. Intervalo válido 1-3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação. Intervalo válido 1-3600.|
|eapolStartPeriodInSeconds|Int32|Especifique o número de segundos a ser aguardado antes de enviar uma mensagem inicial EAPOL (Extensible Authentication Protocol over LAN). Intervalo válido 1-3600.|
|maximumEAPOLStartMessages|Int32|Especifique o número máximo de mensagens de início EAPOL (Protocolo de Autenticação Extensível por LAN) a serem enviadas antes de retornar a falha. Intervalo válido de 1 a 100.|
|maximumAuthenticationFailures|Int32|Especifique as falhas máximas de autenticação permitidas para um conjunto de credenciais. Intervalo válido de 1 a 100.|
|enforce8021X|Booleano|Quando VERDADEIRO, o serviço de configuração automática para redes com fio exige o uso de 802,1X para autenticação de porta. Quando FALSE, 802.1X não é necessário. O valor padrão é FALSE.|
|authenticationBlockPeriodInMinutes|Int32|Especifique a duração para a qual as tentativas de autenticação automática serão impedidas de ocorrer após uma tentativa de autenticação com falha.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de Autenticação Extensível (EAP). Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`. Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Conjunto de cadeias de caracteres|Especifique nomes de certificados de servidor confiáveis.|
|authenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Especifique o método de autenticação. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Especifique o método de autenticação secundário. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Especifique o protocolo de autenticação interna para TTLS EAP. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar TTLS EAP ou PEAP.|
|performServerValidation|Booleano|Quando TRUE, habilita a verificação da identidade do servidor validando o certificado quando o tipo EAP é selecionado como PEAP. Quando FALSE, o certificado não é validado. O valor padrão é TRUE.|
|disableUserPromptForServerValidation|Booliano|Quando TRUE, impede que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP. Quando FALSE, não impede que o usuário seja solicitado. O valor padrão é FALSE.|
|requireCryptographicBinding|Booleano|Quando TRUE, habilita a associação criptográfica quando o tipo EAP é selecionado como PEAP. Quando FALSE, não habilita a associação cryptogrpahic. O valor padrão é TRUE.|
|forceFIPSCompliance|Booleano|Quando TRUE, força a conformidade fips. Quando FALSE, não habilita a conformidade FIPS. O valor padrão é FALSE.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
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
  "authenticationType": "user",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 2,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "secondaryAuthenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
  "id": "ec132acd-2acd-ec13-cd2a-13eccd2a13ec",
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
  "authenticationType": "user",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 2,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "secondaryAuthenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```




