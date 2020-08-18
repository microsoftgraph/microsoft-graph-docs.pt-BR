---
title: tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 369631fc29203c54ef3c63c2cd32df67254c76bf
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791775"
---
# <a name="hardwareinformation-resource-type"></a>tipo de recurso hardwareInformation

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|serialNumber|String|Número de série.|
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
|isSupervised|Boolean|Modo supervisionado do dispositivo|
|isEncrypted|Boolean|Status de criptografia do dispositivo|
|batterySerialNumber|String|O número de série da bateria atual do dispositivo|
|batteryHealthPercentage|Int32|A porcentagem de integridade da bateria atual do dispositivo. Valores válidos de 0 a 100|
|batteryChargeCycles|Int32|O número de ciclos de carga que a bateria atual do dispositivo passou. Valores válidos de 0 a 2147483647|
|isSharedDevice|Booliano|IPad compartilhado|
|sharedDeviceCachedUsers|coleção [sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Todos os usuários no dispositivo Apple compartilhado|
|tpmSpecificationVersion|String|Cadeia de caracteres que especifica a versão da especificação.|
|operatingSystemEdition|String|Cadeia de caracteres que especifica a edição do sistema operacional.|
|deviceFullQualifiedDomainName|String|Retorna o nome de domínio totalmente qualificado do dispositivo (se houver algum). Se o dispositivo não ingressou no domínio, ele retornará uma cadeia de caracteres vazia. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Status do requisito de hardware de segurança baseado em virtualização. Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Status de segurança baseado em virtualização. . Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status do LSA (autoridade do sistema local) . Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|String|Número de compilação do sistema operacional no dispositivo Android|
|operatingSystemProductType|Int32|Int que especifica o produto do sistema operacional Windows. Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 . Valores válidos de 0 a 2147483647|

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
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024
}
```



