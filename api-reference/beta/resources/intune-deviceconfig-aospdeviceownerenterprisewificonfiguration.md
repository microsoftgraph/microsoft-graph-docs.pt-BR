---
title: tipo de recurso aospDeviceOwnerEnterpriseWiFiConfiguration
description: Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo proprietário do dispositivo AOSP a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da1e031af52b8b19c8f6cbd6057998f9f716ca5c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203194"
---
# <a name="aospdeviceownerenterprisewificonfiguration-resource-type"></a>tipo de recurso aospDeviceOwnerEnterpriseWiFiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo proprietário do dispositivo AOSP a se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final.


Herda de [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar aospDeviceOwnerEnterpriseWiFiConfigurations](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-list.md)|[coleção aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Listar propriedades e relações dos [objetos aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Obter aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-get.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Ler propriedades e relações do [objeto aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Criar aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-create.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Crie um [novo objeto aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Excluir aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-delete.md)|Nenhuma|Exclui um [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md).|
|[Atualizar aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-update.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Atualize as propriedades de um [objeto aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|Cadeia de Caracteres|Nome de rede herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|Ssid|Cadeia de Caracteres|Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectAutomatically|Booliano|Conexão automaticamente quando essa rede estiver no intervalo. Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Booliano|Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|wiFiSecurityType|[aospDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-aospdeviceownerwifisecuritytype.md)|Indica se o Wi-Fi de extremidade usa um tipo de segurança baseado em EAP. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md). Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|Cadeia de Caracteres|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|preSharedKeyIsSet|Booliano|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal. Herdado [de aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Indica o tipo de protocolo EAP definido no ponto Wi-Fi (roteador). Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.|
|trustedServerCertificateNames|Conjunto de cadeias de caracteres|Nomes de certificado de servidor confiáveis quando o Tipo de EAP está configurado para EAP-TLS/TTLS/FAST ou PEAP. Esse é o nome comum usado nos certificados emitidos pela ac (autoridade de certificação) confiável. Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e Authenticationmethod é nome de usuário e senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e Authenticationmethod é nome de usuário e senha. Esta coleção pode conter um máximo de 500 elementos. Os valores possíveis são: `none` e `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Cadeia de Caracteres|Habilite a privacidade de identidade (Identidade Externa) quando o Tipo de EAP estiver configurado para EAP-TTLS ou PEAP. A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.|

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
|rootCertificateForServerValidation|[aospDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-aospdeviceownertrustedrootcertificate.md)|Certificado raiz confiável para validação de servidor quando o Tipo de EAP está configurado para EAP-TLS, EAP-TTLS ou PEAP. Esse é o certificado apresentado pelo ponto de extremidade Wi-Fi quando o dispositivo tenta se conectar Wi-Fi ponto de extremidade. O dispositivo (ou usuário) deve aceitar esse certificado para continuar a tentativa de conexão.|
|identityCertificateForClientAuthentication|[aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|Certificado de identidade para autenticação de cliente quando o Tipo de EAP está configurado para EAP-TLS, EAP-TTLS (com Autenticação de Certificado) ou PEAP (com Autenticação de Certificado). Esse é o certificado apresentado pelo cliente ao ponto de extremidade Wi-Fi cliente. O servidor de autenticação que está atrás Wi-Fi ponto de extremidade deve aceitar esse certificado para estabelecer com êxito uma Wi-Fi conexão.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration",
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




