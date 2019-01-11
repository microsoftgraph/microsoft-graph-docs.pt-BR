---
title: tipo de recurso de hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2684f1ff7e7a6407942ac61fae7d45ead16820d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831819"
---
# <a name="hardwareinformation-resource-type"></a>tipo de recurso de hardwareInformation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Informações de hardware de um determinado dispositivo.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|serialNumber|Cadeia de caracteres|Número de série.|
|totalStorageSpace|Int64|Espaço de armazenamento total do dispositivo.|
|freeStorageSpace|Int64|Espaço livre de armazenamento do dispositivo.|
|imei|Cadeia de caracteres|IMEI|
|meid|Cadeia de caracteres|MEID|
|fabricante|Cadeia de caracteres|Fabricante do dispositivo|
|modelo|Cadeia de caracteres|Modelo do dispositivo|
|phoneNumber|Cadeia de caracteres|Número de telefone do dispositivo|
|subscriberCarrier|Cadeia de caracteres|Operadora de assinante do dispositivo|
|cellularTechnology|Cadeia de caracteres|Tecnologia de celular do dispositivo|
|wifiMac|Cadeia de caracteres|Endereço MAC WiFi do dispositivo|
|operatingSystemLanguage|Cadeia de caracteres|Idioma do sistema operacional do dispositivo|
|isSupervised|Booliano|Supervisionadas modo do dispositivo|
|isEncrypted|Booliano|Status de criptografia do dispositivo|
|isSharedDevice|Booliano|IPad compartilhado|
|sharedDeviceCachedUsers|coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Todos os usuários no compartilhados dispositivo Apple|
|tpmSpecificationVersion|Cadeia de caracteres|Cadeia de caracteres que especifica a versão de especificação.|
|operatingSystemEdition|Cadeia de caracteres|Cadeia de caracteres que especifica a edição do sistema operacional.|
|deviceFullQualifiedDomainName|Cadeia de caracteres|Retorna o nome de domínio totalmente qualificado do dispositivo (se houver). Se o dispositivo não está associado ao domínio, ele retornará uma sequência vazia. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Status de requisito de hardware de segurança baseada em virtualização. Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Status de segurança baseada em virtualização. . Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status do protetor de credencial sistema autoridade (LSA) local. . Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|

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





