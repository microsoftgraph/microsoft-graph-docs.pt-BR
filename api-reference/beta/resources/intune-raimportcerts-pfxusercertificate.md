---
title: tipo de recurso pfxUserCertificate
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b77d5d4c36e7ac968a7c1ce4cf1a0645ce87153
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272077"
---
# <a name="pfxusercertificate-resource-type"></a>tipo de recurso pfxUserCertificate

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar pfxUserCertificates](../api/intune-raimportcerts-pfxusercertificate-list.md)|coleção [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Listar Propriedades e relações dos objetos [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Obter pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-get.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Leia as propriedades e as relações do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Criar pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-create.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Criar um novo objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Excluir pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-delete.md)|Nenhum|Exclui [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).|
|[Atualizar pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-update.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Atualiza as propriedades de um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tenantId|Guid|Ainda não documentado|
|userId|Guid|Ainda não documentado|
|identificação|String|Ainda não documentado|
|userUpn|String|Ainda não documentado|
|encryptedPfxBlob|String|Ainda não documentado|
|encryptedPfxPassword|String|Ainda não documentado|
|certStartDate|DateTimeOffset|Ainda não documentado|
|certExpirationDate|DateTimeOffset|Ainda não documentado|
|providerName|String|Ainda não documentado|
|encryptionKeyName|String|Ainda não documentado|
|paddingScheme|Int32|Ainda não documentado|
|status|Int32|Ainda não documentado|
|Da intendedpurpose|Int32|Ainda não documentado|
|createdtime|DateTimeOffset|Ainda não documentado|
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




