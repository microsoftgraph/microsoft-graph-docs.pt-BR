---
title: tipo de recurso de managedDeviceCertificateState
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0975049cd7597735a32b646cc5d719b371a5d27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419097"
---
# <a name="manageddevicecertificatestate-resource-type"></a>tipo de recurso de managedDeviceCertificateState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|coleção [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Lista as propriedades e os relacionamentos dos objetos [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Obter managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Leia as propriedades e os relacionamentos do objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Criar managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Crie um novo objeto de [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Excluir managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Nenhum|Exclui um [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[Atualizar managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Atualize as propriedades de um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Plataforma do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|Uso da chave. Os valores possíveis são: `keyEncipherment` e `digitalSignature`.|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Unidades do período de validade. Os valores possíveis são: `days`, `months`, `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|Estado de emissão. Os valores possíveis são: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|Provedor de armazenamento de chave. Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Formato de nome de entidade. Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Formato de nome alternativo da entidade. Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Revogar o status. Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|String|Nome de exibição de perfil de certificado|
|deviceDisplayName|Cadeia de caracteres|Nome de exibição do dispositivo|
|userDisplayName|String|Nome de exibição do usuário|
|certificateExpirationDateTime|DateTimeOffset|Data de expiração de certificado|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Última alteração de estado de emissão de certificado|
|lastCertificateStateChangeDateTime|DateTimeOffset|Última alteração de estado de emissão de certificado|
|certificateIssuer|String|Emissor|
|certificateThumbprint|String|Impressão digital|
|Número_serial_do_certificado|String|Número de série|
|certificateKeyLength|Int32|Comprimento da chave|
|certificateEnhancedKeyUsage|String|Uso estendido de chave|
|certificateValidityPeriod|Int32|Período de validade|
|certificateSubjectNameFormatString|String|Sequência de formato de nome de entidade para formatos de nome de entidade personalizada|
|certificateSubjectAlternativeNameFormatString|String|Sequência de formato de nome alternativo de entidade para formatos personalizados|
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




