---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: luleonpla
ms.openlocfilehash: f73cb515ce400762771c7553f6f668c295645b90
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965067"
---
# <a name="selfsignedcertificate-resource-type"></a>Tipo de recurso selfSignedCertificate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém a parte pública de um certificado de assinatura. É o tipo de retorno da ação [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md). Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.

## <a name="properties"></a>Propriedades
Propriedade|Tipo|Descrição
----|--|---
|customKeyIdentifier|Binária| Identificador de chave personalizada |
| displayName | Cadeia de caracteres | O nome amigável da chave. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z". |
|keyId|Guid|O identificador exclusivo (GUID) da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria esta aparência: "2014-01-01T00:00:00Z". |
|tipo|Cadeia de caracteres|O tipo de credencial de chave. "AsymmetricX509Cert".|
|usage|Cadeia de caracteres|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada. Por exemplo, "Verificar".|
|chave|Binário| O valor da credencial de chave. Deve ser um valor codificado de base-64. |
|thumbprint| Cadeia de caracteres | O valor de impressão digital da chave.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "binary",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "binary",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

