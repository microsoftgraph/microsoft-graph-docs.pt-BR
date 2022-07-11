---
title: Tipo de recurso hardwareInformation
description: Informações de hardware de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09dde616eee8d4740f33499baebcf784967ad93d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670313"
---
# <a name="hardwareinformation-resource-type"></a>Tipo de recurso hardwareInformation

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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
|cellularTechnology|Cadeia de Caracteres|Tecnologia de celular do dispositivo|
|wifiMac|Cadeia de caracteres|Endereço MAC WiFi do dispositivo|
|operatingSystemLanguage|Cadeia de Caracteres|Idioma do sistema operacional do dispositivo|
|isSupervised|Boolean|Modo supervisionado do dispositivo|
|isEncrypted|Boolean|Status de criptografia do dispositivo|
|batterySerialNumber|Cadeia de Caracteres|O número de série da bateria atual do dispositivo|
|batteryHealthPercentage|Int32|O percentual de integridade da bateria atual do dispositivo. Valores válidos de 0 a 100|
|batteryChargeCycles|Int32|O número de ciclos de carga que a bateria atual do dispositivo passou. Valores válidos de 0 a 2147483647|
|isSharedDevice|Booliano|iPad compartilhado|
|sharedDeviceCachedUsers|[Coleção sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)|Todos os usuários no dispositivo Apple compartilhado|
|tpmSpecificationVersion|Cadeia de caracteres|Cadeia de caracteres que especifica a versão de especificação.|
|operatingSystemEdition|Cadeia de Caracteres|Cadeia de caracteres que especifica a edição do sistema operacional.|
|deviceFullQualifiedDomainName|Cadeia de caracteres|Retorna o nome de domínio totalmente qualificado do dispositivo (se houver). Se o dispositivo não estiver ingressado no domínio, ele retornará uma cadeia de caracteres vazia. |
|deviceGuardVirtualizationBasedSecurityHardwareRequirementState|[deviceGuardVirtualizationBasedSecurityHardwareRequirementState](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|Status do requisito de hardware de segurança baseado em virtualização. Os valores possíveis são: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.|
|deviceGuardVirtualizationBasedSecurityState|[deviceGuardVirtualizationBasedSecurityState](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|Status de segurança baseado em virtualização. . Os valores possíveis são: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.|
|deviceGuardLocalSystemAuthorityCredentialGuardState|[deviceGuardLocalSystemAuthorityCredentialGuardState](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|Status do proteção de credencial da LSA (Autoridade do Sistema Local). . Os valores possíveis são: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.|
|osBuildNumber|Cadeia de caracteres|Número de build do sistema operacional no dispositivo Android|
|operatingSystemProductType|Int32|Int que especifica o ProductType do Sistema Operacional Windows. Mais detalhes aqui https://go.microsoft.com/fwlink/?linkid=2126950. Valores válidos de 0 a 2147483647|
|ipAddressV4|Cadeia de Caracteres|IPAddressV4|
|subnetAddress|Cadeia de Caracteres|SubnetAddress|
|esimIdentifier|Cadeia de Caracteres|Identificador eSIM|
|systemManagementBIOSVersion|Cadeia de Caracteres|Versão do BIOS conforme relatado pelo SMBIOS|
|tpmManufacturer|Cadeia de caracteres|As informações de identificação que nomeia exclusivamente o fabricante do TPM|
|tpmVersion|Cadeia de caracteres|A versão do TPM, conforme especificado pelo fabricante|
|wiredIPv4Addresses|Conjunto de cadeias de caracteres|Uma lista de endereços IPv4 com fio. A frequência de atualização (o atraso máximo para a alteração do valor da propriedade a ser sincronizada do dispositivo para o armazenamento em nuvem) dessa propriedade é diária. Observe que essa propriedade atualmente tem suporte apenas em dispositivos em execução no Windows.|
|batteryLevelPercentage|Duplo|O nível da bateria, entre 0,0 e 100, ou nulo se o nível da bateria não puder ser determinado. A frequência de atualização dessa propriedade é por check-in. Observe que essa propriedade só tem suporte em dispositivos que executam o iOS 5.0 e posterior e está disponível somente quando o direito de acesso às Informações do Dispositivo é obtido. Valores válidos de 0 a 100|
|residentUsersCount|Int32|O número de usuários atualmente neste dispositivo ou nulo (padrão) se o valor dessa propriedade não puder ser determinado. A frequência de atualização dessa propriedade é por check-in. Observe que essa propriedade tem suporte apenas em dispositivos que executam o iOS 13.4 e posterior e está disponível somente quando o direito de acesso às Informações do Dispositivo é obtido. Valores válidos de 0 a 2147483647|
|productName|Cadeia de caracteres|O nome do produto, por exemplo, iPad8,12 etc. A frequência de atualização dessa propriedade é semanal. Observe que essa propriedade tem suporte apenas em dispositivos iOS/MacOS e está disponível somente quando o direito de acesso às Informações do Dispositivo é obtido.|
|deviceLicensingStatus|[deviceLicensingStatus](../resources/intune-devices-devicelicensingstatus.md)|Status de licenciamento de assinatura baseado em dispositivo. A frequência de atualização dessa propriedade é diária. Observe que essa propriedade atualmente tem suporte apenas para licenciamento de assinatura baseada em dispositivo baseado no Windows. Caso não haja suporte, o valor será definido como desconhecido (-1). Os valores possíveis são: `licenseRefreshStarted`, `licenseRefreshPending`, `deviceIsNotAzureActiveDirectoryJoined`, `verifyingMicrosoftDeviceIdentity`, `deviceIdentityVerificationFailed`, `verifyingMirosoftAccountIdentity`, `mirosoftAccountVerificationFailed`, `acquiringDeviceLicense`, `refreshingDeviceLicense`, `deviceLicenseRefreshSucceed`, `deviceLicenseRefreshFailed`, `removingDeviceLicense`, `deviceLicenseRemoveSucceed`, `deviceLicenseRemoveFailed`, `unknownFutureValue`, `unknown`.|
|deviceLicensingLastErrorCode|Int32|Um código de erro padrão que indica o último erro ou 0 indicando nenhum erro (padrão). A frequência de atualização dessa propriedade é diária. Observe que essa propriedade atualmente tem suporte apenas para licenciamento de assinatura baseada em dispositivo baseado no Windows. Valores válidos de 0 a 2147483647|
|deviceLicensingLastErrorDescription|Cadeia de Caracteres|Mensagem de texto de erro como uma descripição para deviceLicensingLastErrorCode. A frequência de atualização dessa propriedade é diária. Observe que essa propriedade atualmente tem suporte apenas para licenciamento de assinatura baseada em dispositivo baseado no Windows.|

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
  "tpmVersion": "String",
  "wiredIPv4Addresses": [
    "String"
  ],
  "batteryLevelPercentage": "4.2",
  "residentUsersCount": 1024,
  "productName": "String",
  "deviceLicensingStatus": "String",
  "deviceLicensingLastErrorCode": 1024,
  "deviceLicensingLastErrorDescription": "String"
}
```




