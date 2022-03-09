---
title: tipo de recurso aospDeviceOwnerPkcsCertificateProfile
description: Perfil de certificado PKCS do proprietário do dispositivo AOSP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f994f864e4c3a0fa37e81b361587d7474ac1357c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378726"
---
# <a name="aospdeviceownerpkcscertificateprofile-resource-type"></a>tipo de recurso aospDeviceOwnerPkcsCertificateProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de certificado PKCS do proprietário do dispositivo AOSP


Herda [de aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar aospDeviceOwnerPkcsCertificateProfiles](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-list.md)|[coleção aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Listar propriedades e relações dos [objetos aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Obter aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-get.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Leia propriedades e relações do [objeto aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Criar aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-create.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Crie um novo [objeto aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|
|[Excluir aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-delete.md)|Nenhuma|Exclui um [aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md).|
|[Atualizar aospDeviceOwnerPkcsCertificateProfile](../api/intune-deviceconfig-aospdeviceownerpkcscertificateprofile-update.md)|[aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md)|Atualize as propriedades de um [objeto aospDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-aospdeviceownerpkcscertificateprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|certificationAuthority|Cadeia de caracteres|Autoridade de Certificação PKCS|
|certificationAuthorityName|String|Nome da autoridade de certificação PKCS|
|certificationAuthorityType|[deviceManagementCertificationAuthority](../resources/intune-deviceconfig-devicemanagementcertificationauthority.md)|Tipo de autoridade de certificação. Os valores possíveis são: `notConfigured`, `microsoft`, `digiCert`.|
|certificateTemplateName|Cadeia de caracteres|Nome do modelo de certificado PKCS|
|subjectAlternativeNameFormatString|String|Cadeia de caracteres personalizada que define o AAD Atributo.|
|subjectNameFormatString|String|Formato personalizado a ser usado com SubjectNameFormat = Custom. Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|Certificado de armazenamento de destino. Os valores possíveis são: `user` e `machine`.|
|customSubjectAlternativeNames|[Coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)|Nome alternativo de assunto personalizado Configurações. Esta coleção pode conter um máximo de 500 elementos.|

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
|managedDeviceCertificateStates|[coleção managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Estado do certificado para dispositivos. Essa coleção pode conter um máximo de 2147483647 elementos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerPkcsCertificateProfile",
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
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificationAuthorityType": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String",
  "subjectNameFormatString": "String",
  "certificateStore": "String",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ]
}
```




