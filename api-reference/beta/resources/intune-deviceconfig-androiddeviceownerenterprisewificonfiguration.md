---
title: Tipo de recurso androidDeviceOwnerEnterpriseWiFiConfiguration
description: Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo Android Proprietário do Dispositivo a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb6656a2d8e38629b3f80be6b5565724a5350b31
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858318"
---
# <a name="androiddeviceownerenterprisewificonfiguration-resource-type"></a>Tipo de recurso androidDeviceOwnerEnterpriseWiFiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo Android Proprietário do Dispositivo a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.


Herda de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerEnterpriseWiFiConfigurations](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-list.md)|[coleção androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Listar propriedades e relações dos [objetos androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Obter androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-get.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Ler propriedades e relações do objeto [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Criar androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-create.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Crie um novo [objeto androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Excluir androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-delete.md)|Nenhum|Exclui um [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).|
|[Atualizar androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-update.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Atualize as propriedades de um [objeto androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|String|Nome de rede herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|Ssid|String|Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|connectAutomatically|Booliano|Conexão automaticamente quando essa rede estiver no intervalo. Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Booliano|Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|wiFiSecurityType|[androidDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|Indica se o Wi-Fi de extremidade usa um tipo de segurança baseado em EAP. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md). Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|String|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|preSharedKeyIsSet|Booliano|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Especifique a configuração de proxy Wi-Fi configuração. Os valores possíveis incluem nenhum, manual e automático. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md). Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Especifique o endereço IP do servidor proxy. Android documentação não especifica IPv4 ou IPv6. Por exemplo: 192.168.1.1. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyManualPort|Int32|Especifique a porta do servidor proxy. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|Especifique a URL de script de configuração do servidor proxy. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyExclusionList|String|Lista de hosts a serem excluídos usando o proxy em conexões. Esses hosts podem usar caracteres curinga, como *.example.com. Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.|
|trustedServerCertificateNames|Coleção de cadeias de caracteres|Nomes de certificado de servidor confiáveis quando o Tipo de EAP está configurado para EAP-TLS/TTLS/FAST ou PEAP. Esse é o nome comum usado nos certificados emitidos pela ac (autoridade de certificação) confiável. Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e Authenticationmethod é nome de usuário e senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e Authenticationmethod é nome de usuário e senha. Os valores possíveis são: `none` e `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Habilite a privacidade de identidade (Identidade Externa) quando o Tipo de EAP estiver configurado para EAP-TTLS ou PEAP. A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|rootCertificateForServerValidation|[androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md)|Certificado raiz confiável para validação de servidor quando o Tipo de EAP está configurado para EAP-TLS, EAP-TTLS ou PEAP. Esse é o certificado apresentado pelo ponto de extremidade Wi-Fi quando o dispositivo tenta se conectar Wi-Fi ponto de extremidade. O dispositivo (ou usuário) deve aceitar esse certificado para continuar a tentativa de conexão.|
|identityCertificateForClientAuthentication|[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)|Certificado de identidade para autenticação de cliente quando o Tipo de EAP está configurado para EAP-TLS, EAP-TTLS (com Autenticação de Certificado) ou PEAP (com Autenticação de Certificado). Esse é o certificado apresentado pelo cliente ao ponto de extremidade Wi-Fi cliente. O servidor de autenticação que está atrás Wi-Fi ponto de extremidade deve aceitar esse certificado para estabelecer com êxito uma Wi-Fi conexão.|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Configurações de nível de locatário para as Credenciais Derivadas a serem usadas para autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "preSharedKey": "String",
  "preSharedKeyIsSet": true,
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "proxyExclusionList": "String",
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




