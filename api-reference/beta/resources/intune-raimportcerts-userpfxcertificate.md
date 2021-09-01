---
title: Tipo de recurso userPFXCertificate
description: Entidade que encapsula todas as informações necessárias para os certificados PFX de um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92764f6fd5fa717698ae2ed629a80e9035274888
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757892"
---
# <a name="userpfxcertificate-resource-type"></a>Tipo de recurso userPFXCertificate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que encapsula todas as informações necessárias para os certificados PFX de um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[Coleção userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Listar propriedades e relações dos [objetos userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Obter userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Leia propriedades e relações do [objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Criar userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Crie um novo [objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Excluir userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Nenhum(a)|Exclui um [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Atualizar userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Atualize as propriedades de [um objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do certificado PFX.|
|thumbprint|Cadeia de caracteres|Impressão digital SHA-1 do certificado PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Finalidade pretendido do certificado do ponto de vista da implantação. Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário do certificado PFX.|
|startDateTime|DateTimeOffset|Data/hora de início da validade do certificado.|
|expirationDateTime|DateTimeOffset|Data/hora de validade do certificado.|
|providerName|Cadeia de caracteres|Provedor de criptografia usado para criptografar esse blob.|
|keyName|Cadeia de caracteres|Nome da chave (dentro do provedor) usada para criptografar o blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Esquema de preenchimento usado pelo provedor durante a criptografia/descriptografia. Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binário|Blob PFX criptografado.|
|encryptedPfxPassword|Cadeia de caracteres|Senha PFX criptografada.|
|createdDateTime|DateTimeOffset|Data/hora em que esse certificado PFX foi importado.|
|lastModifiedDateTime|DateTimeOffset|Data/hora em que esse certificado PFX foi modificado pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



