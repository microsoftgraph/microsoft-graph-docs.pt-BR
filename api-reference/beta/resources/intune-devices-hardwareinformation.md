---
title: Tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a01c6b27d57947d14ba907a0d2dcf662b5e57f79
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799793"
---
# <a name="hardwareinformation-resource-type"></a>Tipo de recurso hardwareInformation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|serialNumber|String|Número de série.|
|totalStorageSpace|Int64|Espaço de armazenamento total do dispositivo.|
|freeStorageSpace|Int64|Espaço de armazenamento gratuito do dispositivo.|
|imei|String|IMEI|
|meid|String|MEID|
|fabricante|String|Fabricante do dispositivo|
|modelo|String|Modelo do dispositivo|
|phoneNumber|String|Número de telefone do dispositivo|
|subscriberCarrier|String|Operadora de assinante do dispositivo|
|cellularTechnology|Cadeia de caracteres|Tecnologia celular do dispositivo|
|wifiMac|Cadeia de caracteres|Endereço MAC WiFi do dispositivo|
|operatingSystemLanguage|Cadeia de caracteres|Idioma do sistema operacional do dispositivo|
|isSupervised|Boolean|Modo supervisionado do dispositivo|
|isEncrypted|Boolean|Status de criptografia do dispositivo|
|batterySerialNumber|Cadeia de caracteres|O número de série da bateria atual do dispositivo|
|batteryHealthPercentage|Int32|A porcentagem de saúde da bateria atual do dispositivo. Valores válidos de 0 a 100|
|batteryChargeCycles|Int32|O número de ciclos de carga que a bateria atual do dispositivo passou. Valores válidos de 0 a 2147483647|
|isSharedDevice|Boleano|Dados iPad|
|sharedDeviceCachedUsers|[Coleção sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Todos os usuários no dispositivo Apple compartilhado|
|tpmSpecificationVersion|Cadeia de caracteres|Cadeia de caracteres que especifica a versão de especificação.|
|operatingSystemEdition|Cadeia de caracteres|Cadeia de caracteres que especifica a edição do sistema operacional.|
|deviceFullQualifiedDomainName|Cadeia de caracteres|Retorna o nome de domínio totalmente qualificado do dispositivo (se for o caso). Se o dispositivo não for ingressado no domínio, ele retornará uma cadeia de caracteres vazia. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Status do requisito de hardware de segurança baseado em virtualização. Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Status de segurança baseado em virtualização. . Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status do proteção de credenciais da Autoridade de Sistema Local (LSA). . Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|Cadeia de caracteres|Número de com build do sistema operacional no dispositivo Android|
|operatingSystemProductType|Int32|Int que especifica o Windows ProductType do Sistema Operacional. Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950 . Valores válidos de 0 a 2147483647|
|ipAddressV4|Cadeia de caracteres|IPAddressV4|
|subnetAddress|Cadeia de caracteres|SubnetAddress|
|esimIdentifier|Cadeia de caracteres|Identificador eSIM|
|systemManagementBIOSVersion|Cadeia de caracteres|Versão do BIOS conforme relatado por SMBIOS|
|tpmManufacturer|Cadeia de caracteres|As informações de identificação que nomeia exclusivamente o fabricante do TPM|
|tpmVersion|Cadeia de caracteres|A versão do TPM, conforme especificado pelo fabricante|

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
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String"
}
```



