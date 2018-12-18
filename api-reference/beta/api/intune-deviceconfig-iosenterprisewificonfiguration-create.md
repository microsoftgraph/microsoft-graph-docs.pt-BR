---
title: Criar iosEnterpriseWiFiConfiguration
description: Crie um novo objeto de iosEnterpriseWiFiConfiguration.
author: tfitzmac
ms.openlocfilehash: 2e11b506df4fde586aa181602e25da4c499ab6bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320696"
---
# <a name="create-iosenterprisewificonfiguration"></a>Criar iosEnterpriseWiFiConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Crie um novo objeto de [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto iosEnterpriseWiFiConfiguration.

A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosEnterpriseWiFiConfiguration.

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
|networkName|String|Herdado de nome de rede de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|SSID|String|Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Boolean|Conecte automaticamente quando esta rede estiver no intervalo. Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Conecte-se quando a rede não está transmitindo seu nome (SSID). Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP. Herdada do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Tipo de proxy para esta conexão Wi-Fi Inherited de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Nome de host DNS ou endereço IP do servidor proxy quando a configuração manual está selecionada. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|Porta do servidor proxy quando a configuração manual está selecionada. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada. Essa URL normalmente é o local do arquivo PAC (configuração automática de Proxy). Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|String|Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal. Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de autenticação extensível (EAP). Indica o tipo de protocolo EAP definir no ponto de extremidade Wi-Fi (roteador). Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|Opção de configuração de EAP-FAST quando EAP-FAST é o tipo de EAP selecionado. Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|String collection|A confiança de nomes de certificado de servidor quando o tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP. Este é o nome comum usado nos certificados emitidos pela sua autoridade de certificação confiável (CA). Se você fornecer essas informações, você poderá ignorar a caixa de diálogo de confiança dinâmico que é exibida em dispositivos dos usuários finais quando eles se conectam à rede Wi-Fi.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Método de autenticação quando o tipo de EAP é configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate` e `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método Non-EAP para autenticação quando o tipo de EAP é EAP-TTLS e Authenticationmethod é o nome de usuário e senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Habilitar Privacidade de identidade (identidade externa) quando o tipo de EAP é configurado para EAP - TTLS, EAP - FAST ou PEAP. Essa propriedade mascara os nomes de usuário com o texto inserido. Por exemplo, se você usar 'anonymous', cada usuário que autentica com esta conexão Wi-Fi usando seu nome de usuário real é exibido como 'anonymous'.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





