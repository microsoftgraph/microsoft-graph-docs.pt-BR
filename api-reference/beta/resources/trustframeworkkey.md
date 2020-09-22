---
title: tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia. A estrutura desse recurso segue o formato definido na RFC 7517 seção 4.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7650976a437eb862acd5994d7e1dd14830d5e3b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083929"
---
# <a name="trustframeworkkey-resource-type"></a>tipo de recurso trustFrameworkKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave de criptografia. A estrutura desse recurso segue o formato definido na [RFC 7517 seção 4](https://tools.ietf.org/html/rfc7517#section-4).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| filho | cadeia de caracteres | O identificador exclusivo da chave.   |
| kty | cadeia de caracteres | O parâmetro "KTY" (tipo de chave) identifica a família de algoritmos de criptografia usada com a chave, os valores válidos são RSA, Oct. |
| Use | cadeia de caracteres | O parâmetro "Use" (uso de chave pública) identifica o uso pretendido da chave pública.  O parâmetro "Use" é empregado para indicar se uma chave pública é usada para criptografar os dados ou para verificar a assinatura dos dados. Os valores possíveis são 1. "SIG" (assinatura) 2.  "Enc" (criptografia)   |
| x5c | coleção de cadeias de caracteres | O parâmetro "x5c" (cadeia de certificados X. 509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280). |
| x5t | cadeia de caracteres | O parâmetro "x5t" (impressão digital SHA-1 do certificado 509) é uma impressão digital SHA-1 codificada por base64url (conhecida Digest) da codificação DER de um certificado X. 509 [RFC 5280](https://tools.ietf.org/html/rfc5280). |
| minúscula | cadeia de caracteres | Chave RSA – expoente público |
| d| cadeia de caracteres | Chave RSA-expoente privado. O campo não pode ser lido novamente. |
| n | cadeia de caracteres | Chave RSA-módulo |
| p | cadeia de caracteres | Chave RSA-primeira linha. O campo não pode ser lido novamente. |
| q | cadeia de caracteres | Chave RSA-segundo primo. O campo não pode ser lido novamente. |
| distribuição | cadeia de caracteres | Expoente da chave RSA-First. O campo não pode ser lido novamente. |
| DQ | cadeia de caracteres | Expoente da chave RSA-segundo. O campo não pode ser lido novamente. |
| QI | cadeia de caracteres | O coeficiente de chave RSA. O campo não pode ser lido novamente. |
| f | cadeia de caracteres | Chave simétrica para tipo de chave Oct. O campo não pode ser lido novamente.   |
| nbf | int | Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.) |
| exp | int | Esse valor é um NumericDate, conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissextos.) |



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


