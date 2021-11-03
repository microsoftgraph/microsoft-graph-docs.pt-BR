---
title: Tipo de recurso iosEnterpriseWiFiConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir o dispositivo iOS a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d44ef253fe69e36579ac519412ceaefdefb37799
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696081"
---
# <a name="iosenterprisewificonfiguration-resource-type"></a>Tipo de recurso iosEnterpriseWiFiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações neste perfil, você pode instruir o dispositivo iOS a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.


Herda de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosEnterpriseWiFiConfigurations](../api/intune-deviceconfig-iosenterprisewificonfiguration-list.md)|[Coleção iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Listar propriedades e relações dos [objetos iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Obter iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-get.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Leia propriedades e relações do [objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Criar iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-create.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Crie um novo [objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Excluir iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-delete.md)|Nenhum|Exclui [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).|
|[Atualizar iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-update.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Atualize as propriedades de [um objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|String|Nome da rede Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|ssid|String|Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Booliano|Conexão automaticamente quando essa rede estiver no intervalo. Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Booliano|Conexão quando a rede não estiver transmitindo seu nome (SSID). Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP. Herdado [de iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Tipo de proxy para essa Wi-Fi herdada de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual é selecionada. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|Porta do servidor proxy quando a configuração manual é selecionada. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada. Normalmente, essa URL é o local do arquivo PAC (Configuração Automática de Proxy). Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|disableMacAddressRandomization|Booliano|Se definido como true, força os dispositivos que se conectam usando esse perfil de Wi-Fi para apresentar seu endereço MAC real Wi-Fi em vez de um endereço MAC aleatório. Aplica-se ao iOS 14 e posterior. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|String|Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi. Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de Autenticação Extensível (EAP). Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador). Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|Opção de configuração FAST EAP quando o EAP-FAST é o Tipo EAP selecionado. Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|Coleção de cadeias de caracteres|Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP. Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA). Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método não EAP para autenticação quando Tipo EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Habilita a privacidade de identidade (Identidade Externa) quando o tipo EAP estiver configurado para EAP - TTLS, EAP - FAST ou PEAP. Essa propriedade mascara os nomes de usuário com o texto que você inserir. Por exemplo, se você usar 'anônimo', cada usuário que se autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como "anônimo".|
|usernameFormatString|String|Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar ao wifi|
|passwordFormatString|String|Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação de configuração do dispositivo pelo usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|rootCertificatesForServerValidation|[Coleção iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)|Certificados raiz confiáveis para validação de servidor quando o tipo EAP está configurado para EAP-TLS/TTLS/FAST ou PEAP. Se você fornecer esse valor, não precisará fornecer trustedServerCertificateNames e vice-versa. Esta coleção pode conter um máximo de 500 elementos.|
|identityCertificateForClientAuthentication|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Certificado de Identidade para autenticação do cliente quando Tipo de EAP estiver configurado para EAP-TLS, EAP-TTLS (com Autenticação de Certificado) ou PEAP (com Autenticação de Certificado).|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Configurações de nível de locatário para as Credenciais Derivadas a serem usadas para autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "disableMacAddressRandomization": true,
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "usernameFormatString": "String",
  "passwordFormatString": "String"
}
```



