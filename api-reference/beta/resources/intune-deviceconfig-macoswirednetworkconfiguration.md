---
title: Tipo de recurso macOSWiredNetworkConfiguration
description: Perfil de configuração de rede com fio do MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb0ac5bb77bb8e4cb0b4be3205e72b8e53472c6f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806681"
---
# <a name="macoswirednetworkconfiguration-resource-type"></a>Tipo de recurso macOSWiredNetworkConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de rede com fio do MacOS.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSWiredNetworkConfigurations](../api/intune-deviceconfig-macoswirednetworkconfiguration-list.md)|[Coleção macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|Listar propriedades e relações dos [objetos macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|
|[Obter macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-get.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|Leia propriedades e relações do [objeto macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|
|[Criar macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-create.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|Crie um novo [objeto macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|
|[Excluir macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-delete.md)|Nenhum(a)|Exclui um [macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md).|
|[Atualizar macOSWiredNetworkConfiguration](../api/intune-deviceconfig-macoswirednetworkconfiguration-update.md)|[macOSWiredNetworkConfiguration](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|Atualize as propriedades de [um objeto macOSWiredNetworkConfiguration.](../resources/intune-deviceconfig-macoswirednetworkconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|Cadeia de caracteres|Nome da rede|
|networkInterface|[wiredNetworkInterface](../resources/intune-deviceconfig-wirednetworkinterface.md)|Interface de rede. Os valores possíveis são: `anyEthernet`, `firstActiveEthernet`, `secondActiveEthernet`, `thirdActiveEthernet`, `firstEthernet`, `secondEthernet`, `thirdEthernet`.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Protocolo de Autenticação Extensível (EAP). Indica o tipo de conjunto de protocoloSAP na rede com fio. Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|Opção de configuração FAST EAP quando o EAP-FAST é o Tipo EAP selecionado. Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|Coleção de cadeias de caracteres|Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP. Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA). Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectarem a essa rede com fio.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS. Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|nonEapAuthenticationMethodForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha. Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|enableOuterIdentityPrivacy|Cadeia de caracteres|Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS, EAP-FAST ou PEAP. Essa propriedade mascara os nomes de usuário com o texto que você inserir. Por exemplo, se você usar "anônimo", cada usuário que se autentica com essa rede com fio usando seu nome de usuário real será exibido como "anônimo".|

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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Certificado Raiz Confiável para Validação de Servidor quando Tipo EAP estiver configurado para EAP-TLS/TTLS/FAST ou PEAP.|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Certificado de Identidade para autenticação do cliente quando Tipo de EAP estiver configurado para EAP-TLS, EAP-TTLS (com Autenticação de Certificado) ou PEAP (com Autenticação de Certificado).|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSWiredNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSWiredNetworkConfiguration",
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
  "networkInterface": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "nonEapAuthenticationMethodForEapTtls": "String",
  "enableOuterIdentityPrivacy": "String"
}
```



