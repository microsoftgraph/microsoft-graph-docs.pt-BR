---
title: Tipo de recurso iosPkcsCertificateProfile
description: Perfil de certificado PKCS do iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 884361d418869f0abbab21f56399fe6ddfd1a146
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668171"
---
# <a name="iospkcscertificateprofile-resource-type"></a>Tipo de recurso iosPkcsCertificateProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de certificado PKCS do iOS.


Herda de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosPkcsCertificateProfiles](../api/intune-deviceconfig-iospkcscertificateprofile-list.md)|[Coleção iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|Listar propriedades e relações dos objetos [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .|
|[Obter iosPkcsCertificateProfile](../api/intune-deviceconfig-iospkcscertificateprofile-get.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|Ler propriedades e relações do objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .|
|[Criar iosPkcsCertificateProfile](../api/intune-deviceconfig-iospkcscertificateprofile-create.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|Crie um novo [objeto iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .|
|[Excluir iosPkcsCertificateProfile](../api/intune-deviceconfig-iospkcscertificateprofile-delete.md)|Nenhum|Exclui um [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).|
|[Atualizar iosPkcsCertificateProfile](../api/intune-deviceconfig-iospkcscertificateprofile-update.md)|[iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md)|Atualize as propriedades de um [objeto iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .|

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
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|renewalThresholdPercentage|Int32|Percentual de limite de renovação de certificado. Valores válidos de 1 a 99 Herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|
|subjectNameFormat|[appleSubjectNameFormat](../resources/intune-deviceconfig-applesubjectnameformat.md)|Formato de nome da entidade do certificado. Herdado [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md). Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Tipo de Nome Alternativo da Entidade de Certificado. Herdado [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md). Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificateValidityPeriodValue|Int32|Valor do período de validade do certificado. Herdado [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Dimensionar para o período de validade do certificado. Herdado [de iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md). Os valores possíveis são: `days`, `months`, `years`.|
|certificationAuthority|Cadeia de caracteres|Autoridade de Certificação PKCS.|
|certificationAuthorityName|Cadeia de caracteres|Nome da Autoridade de Certificação PKCS.|
|certificateTemplateName|Cadeia de caracteres|Nome do modelo de certificado PKCS.|
|subjectAlternativeNameFormatString|String|Cadeia de caracteres personalizada que define o atributo do AAD.|
|subjectNameFormatString|Cadeia de caracteres|Formato personalizado a ser usado com SubjectNameFormat = Custom. Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|
|Certificatestore|[Certificatestore](../resources/intune-shared-certificatestore.md)|Certificado do repositório de destino. Os valores possíveis são: `user` e `machine`.|
|customSubjectAlternativeNames|[coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)|Configurações de Nome Alternativo da Entidade Personalizada. Esta coleção pode conter um máximo de 500 elementos.|

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
|managedDeviceCertificateStates|[coleção managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Estado do certificado para dispositivos. Essa coleção pode conter um máximo de 2147483647 elementos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosPkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
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




