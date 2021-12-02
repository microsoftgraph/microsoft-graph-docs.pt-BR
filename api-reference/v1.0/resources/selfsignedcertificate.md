---
title: Tipo de recurso selfSignedCertificate
description: Contém informações sobre a parte pública de um certificado de assinatura.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: alamaral
ms.openlocfilehash: 6d17c2c1d41733423c1ef3d892df05c442b5ac71
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266398"
---
# <a name="selfsignedcertificate-resource-type"></a>Tipo de recurso selfSignedCertificate

Namespace: microsoft.graph

Contém a parte pública de um certificado de assinatura. 

Esse tipo de recurso é o tipo de retorno da [ação addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md) Os provedores de serviços usam a parte pública do certificado de assinatura para validar o emissor do token.

## <a name="properties"></a>Propriedades
Propriedade|Tipo|Descrição
----|--|---
|customKeyIdentifier|Binária| Identificador de chave personalizado. |
| displayName | Cadeia de caracteres | O nome amigável da chave. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|keyId|Guid|O identificador exclusivo (GUID) da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
|type|Cadeia de caracteres|O tipo de credencial de chave. "AsymmetricX509Cert".|
|usage|String|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada. O valor possível é `Verify` .|
|chave|Binário| O valor da credencial de chave. Deve ser um valor codificado da Base-64. |
|thumbprint| Cadeia de caracteres | O valor de impressão digital da chave.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
  "@odata.type": "#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "String (Binary)",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "String (Binary)",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "thumbprint": "String",
  "type": "String",
  "usage": "String"
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

