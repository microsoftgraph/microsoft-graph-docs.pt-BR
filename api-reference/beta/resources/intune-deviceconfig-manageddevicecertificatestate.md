---
title: Tipo de recurso managedDeviceCertificateState
description: Ainda não documentado
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d8ccb42118e611903484b30d43b6017c044c6ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086810"
---
# <a name="manageddevicecertificatestate-resource-type"></a>Tipo de recurso managedDeviceCertificateState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[coleção managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Listar propriedades e relações dos [objetos managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Obter managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Leia propriedades e relações do [objeto managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Criar managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Crie um novo [objeto managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Excluir managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Nenhum|Exclui [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[Atualizar managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Atualize as propriedades de [um objeto managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|devicePlatform|[devicePlatformType](../resources/intune-deviceconfig-deviceplatformtype.md)|Plataforma do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.|
|certificateKeyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|Uso de chave. Os valores possíveis são: `keyEncipherment` e `digitalSignature`.|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Unidades de período de validade. Os valores possíveis são: `days`, `months`, `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|Estado de emissão. Os valores possíveis são: `unknown` , , , , , , , , `challengeIssued` `challengeIssueFailed` , `requestCreationFailed` `requestSubmitFailed` , `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` , `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested`|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|Provedor Armazenamento chave. Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Formato de nome do assunto. Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Formato de nome alternativo do assunto. Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Revogar status. Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|Cadeia de Caracteres|Nome de exibição de perfil de certificado|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário|
|certificateExpirationDateTime|DateTimeOffset|Data de expiração do certificado|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Última alteração de estado de emissão de certificado|
|lastCertificateStateChangeDateTime|DateTimeOffset|Última alteração de estado de emissão de certificado|
|certificateIssuer|Cadeia de Caracteres|Emissor|
|certificateThumbprint|Cadeia de Caracteres|Impressão Digital|
|certificateSerialNumber|Cadeia de Caracteres|Número de série|
|certificateKeyLength|Int32|Comprimento de chave|
|certificateEnhancedKeyUsage|Cadeia de Caracteres|Uso estendido de chave|
|certificateValidityPeriod|Int32|Período de validade|
|certificateSubjectNameFormatString|Cadeia de Caracteres|Cadeia de caracteres de formato de nome de assunto para formatos de nome de assunto personalizados|
|certificateSubjectAlternativeNameFormatString|Cadeia de Caracteres|Cadeia de caracteres de formato de nome alternativo de assunto para formatos personalizados|
|certificateIssuanceDateTime|DateTimeOffset|Data de emissão|
|certificateErrorCode|Int32|Código de erro|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```



