---
title: tipo de recurso de userPFXCertificate
description: Entidade que encapsula todas as informações necessárias para PFX certificados um usuário.
localization_priority: Normal
ms.openlocfilehash: 87516c48e53c8117c9efa119fb6cab62844e6b68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809993"
---
# <a name="userpfxcertificate-resource-type"></a>tipo de recurso de userPFXCertificate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que encapsula todas as informações necessárias para PFX certificados um usuário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|coleção [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Lista as propriedades e os relacionamentos dos objetos [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Obter userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Leia as propriedades e os relacionamentos do objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Criar userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Crie um novo objeto de [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Excluir userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Nenhum|Exclui um [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Atualizar userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Atualize as propriedades de um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o certificado PFX.|
|impressão digital|Cadeia de caracteres|SHA-1 impressão digital do certificado PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Destinada a finalidade do ponto de vista da implantação do certificado. Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|Cadeia de caracteres|Nome Principal de usuário do certificado PFX.|
|startDateTime|DateTimeOffset|Data/hora de início da validade do certificado.|
|expirationDateTime|DateTimeOffset|Data de expiração de validade/hora do certificado.|
|providerName|Cadeia de caracteres|Provedor de criptografia usado para criptografar essa blob.|
|nome chave|Cadeia de caracteres|Nome da chave (dentro do provedor) usado para criptografar o blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Esquema usado pelo provedor durante a criptografia/descriptografia de preenchimento. Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binária|Blob PFX criptografado.|
|encryptedPfxPassword|Cadeia de caracteres|Senha PFX criptografada.|
|createdDateTime|DateTimeOffset|Data/hora quando esse certificado PFX foi importado.|
|lastModifiedDateTime|DateTimeOffset|Data/hora da última modificação desse certificado PFX.|

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





