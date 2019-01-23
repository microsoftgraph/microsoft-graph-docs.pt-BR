---
title: tipo de recurso de windows10PkcsCertificateProfile
description: Área de trabalho do Windows 10 e Mobile PKCS perfil de certificado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27379e8c000deda3c5713ef4912fc5bebbefde6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411607"
---
# <a name="windows10pkcscertificateprofile-resource-type"></a>tipo de recurso de windows10PkcsCertificateProfile

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Área de trabalho do Windows 10 e Mobile PKCS perfil de certificado


Herda de [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windows10PkcsCertificateProfiles](../api/intune-deviceconfig-windows10pkcscertificateprofile-list.md)|coleção [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)|Lista as propriedades e os relacionamentos dos objetos [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .|
|[Obter windows10PkcsCertificateProfile](../api/intune-deviceconfig-windows10pkcscertificateprofile-get.md)|[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)|Leia as propriedades e os relacionamentos do objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .|
|[Criar windows10PkcsCertificateProfile](../api/intune-deviceconfig-windows10pkcscertificateprofile-create.md)|[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)|Crie um novo objeto de [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .|
|[Excluir windows10PkcsCertificateProfile](../api/intune-deviceconfig-windows10pkcscertificateprofile-delete.md)|Nenhum|Exclui um [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).|
|[Atualizar windows10PkcsCertificateProfile](../api/intune-deviceconfig-windows10pkcscertificateprofile-update.md)|[windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)|Atualize as propriedades de um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .|

## <a name="properties"></a>Propriedades
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
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificados. Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|
|keyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|subjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|subjectAlternativeNameType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateValidityPeriodValue|Int32|Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md). Os valores possíveis são: `days`, `months`, `years`.|
|certificationAuthority|String|Autoridade de certificação PKCS|
|certificationAuthorityName|String|Nome da autoridade de certificação PKCS|
|certificateTemplateName|String|Nome do modelo de certificado PKCS|
|subjectAlternativeNameFormatString|String|Cadeia de caracteres personalizada que define o atributo AAD.|
|extendedKeyUsages|coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)|Configurações de uso de chave (EKU) estendido. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|managedDeviceCertificateStates|coleção [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Estado de certificado para dispositivos|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10PkcsCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "keyStorageProvider": "String",
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "subjectAlternativeNameFormatString": "String",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ]
}
```




