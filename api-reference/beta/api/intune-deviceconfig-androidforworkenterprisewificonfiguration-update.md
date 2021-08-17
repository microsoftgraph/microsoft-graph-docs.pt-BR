---
title: Atualizar androidForWorkEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto androidForWorkEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05515ec1a68b8d5bc65890f993fafdf4eda3fabe
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262065"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a>Atualizar androidForWorkEnterpriseWiFiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto androidForWorkEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto androidForWorkEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|Cadeia de caracteres|Nome da rede Herdado [do androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|ssid|Cadeia de caracteres|Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos. Herdado [do androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectAutomatically|Boolean|Conexão automaticamente quando essa rede estiver no intervalo. Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede. Herdado [do androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos. Herdado [do androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP. Herdado [de androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md). Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.|
|trustedServerCertificateNames|String collection|Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP. Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA). Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é PEAP e Authenticationmethod é Nome de Usuário e Senha. Os valores possíveis são: `none` e `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Cadeia de caracteres|Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS ou PEAP. A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1635

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1807

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




