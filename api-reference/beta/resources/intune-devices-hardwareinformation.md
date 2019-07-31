---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 874cee0b2b09b3d106d771f2c176ceed3d4d04e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999784"
---
# <a name="hardwareinformation-resource-type"></a>tipo de recurso hardwareInformation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|serialNumber|Cadeia de caracteres|Número de série.|
|totalStorageSpace|Int64|Espaço de armazenamento total do dispositivo.|
|freeStorageSpace|Int64|Espaço de armazenamento livre do dispositivo.|
|imei|String|IMEI|
|meid|String|MEID|
|fabricante|String|Fabricante do dispositivo|
|modelo|String|Modelo do dispositivo|
|phoneNumber|String|Número de telefone do dispositivo|
|subscriberCarrier|String|Operadora do assinante do dispositivo|
|cellularTechnology|String|Tecnologia celular do dispositivo|
|wifiMac|String|Endereço MAC WiFi do dispositivo|
|operatingSystemLanguage|String|Idioma do sistema operacional do dispositivo|
|isSupervised|Booliano|Modo supervisionado do dispositivo|
|isEncrypted|Boolean|Status de criptografia do dispositivo|
|isSharedDevice|Booliano|IPad compartilhado|
|sharedDeviceCachedUsers|coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Todos os usuários no dispositivo Apple compartilhado|
|tpmSpecificationVersion|String|Cadeia de caracteres que especifica a versão da especificação.|
|operatingSystemEdition|String|Cadeia de caracteres que especifica a edição do sistema operacional.|
|deviceFullQualifiedDomainName|String|Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum). Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Status do requisito de hardware de segurança baseado em virtualização. Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Status de segurança baseado em virtualização. . Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status do LSA (autoridade do sistema local) . Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





