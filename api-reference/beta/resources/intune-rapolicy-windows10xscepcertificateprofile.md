---
title: tipo de recurso windows10XSCEPCertificateProfile
description: Perfil de configuração de certificado do Windows X SCEP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8e242140c1a27ed299849158df67c18444ab362
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301436"
---
# <a name="windows10xscepcertificateprofile-resource-type"></a>tipo de recurso windows10XSCEPCertificateProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração de certificado do Windows X SCEP


Herda de [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XSCEPCertificateProfiles](../api/intune-rapolicy-windows10xscepcertificateprofile-list.md)|coleção [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Listar Propriedades e relações dos objetos [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .|
|[Obter windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-get.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Leia as propriedades e as relações do objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .|
|[Criar windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-create.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Criar um novo objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .|
|[Excluir windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-delete.md)|Nenhum|Exclui [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).|
|[Atualizar windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-update.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Atualiza as propriedades de um objeto [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|versão|Int32|Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|String|Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDatetime|DateTimeOffset|O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|Certificado de repositório de destino. Os valores possíveis são: `user` e `machine`.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Dimensionar o período de validade do certificado. Os valores possíveis são: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Valor para o período de validade do certificado|
|extendedKeyUsages|coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)|Configurações de EKU (uso estendido de chave).|
|hashAlgorithm|coleção [HashAlgorithm](../resources/intune-shared-hashalgorithms.md)|Algoritmo de hash do SCEP.|
|keySize|[keySize](../resources/intune-shared-keysize.md)|Tamanho da chave SCEP. Os valores possíveis são: `size1024`, `size2048`, `size4096`.|
|keyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|Provedor de armazenamento de chaves (KSP). Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|uso de|[usos de](../resources/intune-shared-keyusages.md)|Uso da chave do SCEP. Os valores possíveis são: `keyEncipherment` e `digitalSignature`.|
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificado|
|rootCertificateId|Guid|ID de certificado raiz confiável|
|scepServerUrls|Coleção de cadeias de caracteres|URL (s) do servidor de SCEP.|
|subjectAlternativeNameFormats|coleção [windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)|Atributos AAD personalizados.|
|subjectNameFormatString|String|Formato personalizado a ser usado com SubjectNameFormat = Custom. Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XSCEPCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "certificateStore": "String",
  "certificateValidityPeriodScale": "String",
  "certificateValidityPeriodValue": 1024,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "hashAlgorithm": [
    "String"
  ],
  "keySize": "String",
  "keyStorageProvider": "String",
  "keyUsage": "String",
  "renewalThresholdPercentage": 1024,
  "rootCertificateId": "Guid",
  "scepServerUrls": [
    "String"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ],
  "subjectNameFormatString": "String"
}
```




