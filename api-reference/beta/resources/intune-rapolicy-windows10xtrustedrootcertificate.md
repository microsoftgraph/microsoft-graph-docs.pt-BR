---
title: Tipo de recurso windows10XTrustedRootCertificate
description: Windows Perfil de configuração de Certificado Raiz Confiável X
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 244e36858d8f10c164f9d97fe651d5bab96da4d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039627"
---
# <a name="windows10xtrustedrootcertificate-resource-type"></a>Tipo de recurso windows10XTrustedRootCertificate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Perfil de configuração de Certificado Raiz Confiável X


Herda de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XTrustedRootCertificates](../api/intune-rapolicy-windows10xtrustedrootcertificate-list.md)|[Coleção windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Listar propriedades e relações dos [objetos windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Obter windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-get.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Leia propriedades e relações do [objeto windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Criar windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-create.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Crie um novo [objeto windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|
|[Excluir windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-delete.md)|Nenhum|Exclui um [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).|
|[Atualizar windows10XTrustedRootCertificate](../api/intune-rapolicy-windows10xtrustedrootcertificate-update.md)|[windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|Atualize as propriedades de um [objeto windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)|

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
|trustedRootCertificate|Binário|Certificado Raiz Confiável|
|certFileName|Cadeia de Caracteres|Nome do arquivo a ser exibido na interface do usuário.|
|destinationStore|[certificateDestinationStore](../resources/intune-shared-certificatedestinationstore.md)|Local do armazenamento de destino para o Certificado Raiz Confiável. Os valores possíveis são: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XTrustedRootCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "destinationStore": "String"
}
```



