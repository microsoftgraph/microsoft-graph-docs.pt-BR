---
title: Tipo de recurso pfxUserCertificate
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e78b584f908e1c257d645719bb220c05324fc790
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791078"
---
# <a name="pfxusercertificate-resource-type"></a>Tipo de recurso pfxUserCertificate

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar pfxUserCertificates](../api/intune-raimportcerts-pfxusercertificate-list.md)|[Coleção pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Listar propriedades e relações dos objetos [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Obter pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-get.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Leia propriedades e relações do objeto [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Criar pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-create.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Crie um novo [objeto pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Excluir pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-delete.md)|Nenhum(a)|Exclui um [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).|
|[Atualizar pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-update.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Atualize as propriedades de um [objeto pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tenantId|Guid|Ainda não documentado|
|userId|Guid|Ainda não documentado|
|thumbprint|String|Ainda não documentado|
|userUpn|String|Ainda não documentado|
|encryptedPfxBlob|String|Ainda não documentado|
|encryptedPfxPassword|String|Ainda não documentado|
|certStartDate|DateTimeOffset|Ainda não documentado|
|certExpirationDate|DateTimeOffset|Ainda não documentado|
|providerName|String|Ainda não documentado|
|encryptionKeyName|String|Ainda não documentado|
|paddingScheme|Int32|Ainda não documentado|
|status|Int32|Ainda não documentado|
|intendedPurpose|Int32|Ainda não documentado|
|createdTime|DateTimeOffset|Ainda não documentado|
|isDeleted|Booliano|Ainda não documentado|
|lastModifiedTime|DateTimeOffset|Ainda não documentado|
|eTag|String|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxUserCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "Guid",
  "userId": "Guid",
  "thumbprint": "String",
  "userUpn": "String",
  "encryptedPfxBlob": "String",
  "encryptedPfxPassword": "String",
  "certStartDate": "String (timestamp)",
  "certExpirationDate": "String (timestamp)",
  "providerName": "String",
  "encryptionKeyName": "String",
  "paddingScheme": 1024,
  "status": 1024,
  "intendedPurpose": 1024,
  "createdTime": "String (timestamp)",
  "isDeleted": true,
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String"
}
```



