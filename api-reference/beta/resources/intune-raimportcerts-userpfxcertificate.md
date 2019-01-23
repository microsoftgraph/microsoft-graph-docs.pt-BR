---
title: tipo de recurso de userPFXCertificate
description: Entidade que encapsula todas as informações necessárias para PFX certificados um usuário.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 95ae97b44a82d5ec87e3e2622a519debcfd8d7c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406035"
---
# <a name="userpfxcertificate-resource-type"></a>tipo de recurso de userPFXCertificate

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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
|id|String|Identificador exclusivo para o certificado PFX.|
|impressão digital|String|SHA-1 impressão digital do certificado PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Destinada a finalidade do ponto de vista da implantação do certificado. Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|Nome Principal de usuário do certificado PFX.|
|startDateTime|DateTimeOffset|Data/hora de início da validade do certificado.|
|expirationDateTime|DateTimeOffset|Data de expiração de validade/hora do certificado.|
|providerName|String|Provedor de criptografia usado para criptografar essa blob.|
|nome chave|String|Nome da chave (dentro do provedor) usado para criptografar o blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Esquema usado pelo provedor durante a criptografia/descriptografia de preenchimento. Os possíveis valores são: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binária|Blob PFX criptografado.|
|encryptedPfxPassword|String|Senha PFX criptografada.|
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




