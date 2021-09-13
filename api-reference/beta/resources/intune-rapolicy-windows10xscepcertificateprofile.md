---
title: Tipo de recurso windows10XSCEPCertificateProfile
description: Windows Perfil de configuração do certificado X SCEP
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 95d09a6ad4233b33cfc61567d474f90d84175e51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039620"
---
# <a name="windows10xscepcertificateprofile-resource-type"></a>Tipo de recurso windows10XSCEPCertificateProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Perfil de configuração do certificado X SCEP


Herda do [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XSCEPCertificateProfiles](../api/intune-rapolicy-windows10xscepcertificateprofile-list.md)|[Coleção windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Listar propriedades e relações dos [objetos windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|
|[Obter windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-get.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Leia propriedades e relações do [objeto windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|
|[Criar windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-create.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Crie um novo [objeto windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|
|[Excluir windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-delete.md)|Nenhum|Exclui um [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md).|
|[Atualizar windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-update.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|Atualize as propriedades de um [objeto windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|versão|Int32|Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|Cadeia de caracteres|Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|Cadeia de caracteres|Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String collection|Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|Certificado de armazenamento de destino. Os valores possíveis são: `user` e `machine`.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Dimensione para o Período de Validade do Certificado. Os valores possíveis são: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|Valor do Período de Validade do Certificado|
|extendedKeyUsages|[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)|Configurações de Uso de Chave Estendida (EKU).|
|hashAlgorithm|[Coleção hashAlgorithms](../resources/intune-shared-hashalgorithms.md)|Algoritmo de hash SCEP.|
|keySize|[keySize](../resources/intune-shared-keysize.md)|Tamanho da chave SCEP. Os valores possíveis são: `size1024`, `size2048`, `size4096`.|
|keyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|KSP (Provedor Armazenamento chave). Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|keyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|Uso da chave SCEP. Os valores possíveis são: `keyEncipherment` e `digitalSignature`.|
|renewalThresholdPercentage|Int32|Porcentagem de limite de renovação de certificado|
|rootCertificateId|Guid|ID de certificado raiz confiável|
|scepServerUrls|String collection|Url(s) do servidor SCEP.|
|subjectAlternativeNameFormats|[Coleção windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md)|Atributos personalizados do AAD.|
|subjectNameFormatString|Cadeia de Caracteres|Formato personalizado a ser usado com SubjectNameFormat = Custom. Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

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



