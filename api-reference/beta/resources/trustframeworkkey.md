---
title: Tipo de recurso trustFrameworkKey
description: Representa um JWK (JSON Web Key). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na RFC 7517 Seção 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b50e82748db6c0c26252ce6b79290781fa88819b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945631"
---
# <a name="trustframeworkkey-resource-type"></a>Tipo de recurso trustFrameworkKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um JWK (JSON Web Key). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na [RFC 7517 Seção 4](https://tools.ietf.org/html/rfc7517#section-4).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| kid | cadeia de caracteres | O identificador exclusivo da chave.   |
| kty | Cadeia de caracteres | O **parâmetro kty** (tipo de chave) identifica a família de algoritmos criptográficos usados com a chave, Os valores válidos são `rsa` , `oct` . |
| use | Cadeia de caracteres | O **parâmetro use** (uso de chave pública) identifica o uso pretendido da chave pública.  O **parâmetro** use é empregado para indicar se uma chave pública é usada para criptografar dados ou verificar a assinatura em dados. Os valores possíveis são: `sig` (assinatura), `enc` (criptografia)  |
| x5c | coleção de cadeias de caracteres | O **parâmetro x5c** (cadeia de certificados X.509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280](https://tools.ietf.org/html/rfc5280). |
| x5t | cadeia de caracteres | O **parâmetro x5t** (X.509 certificate SHA-1 thumbprint) é uma impressão digital SHA-1 codificada com base64url (a.k.a. digest) da codificação DER de um certificado X.509 [RFC 5280](https://tools.ietf.org/html/rfc5280). |
| e | cadeia de caracteres | CHAVE RSA - expoente público |
| d| cadeia de caracteres | CHAVE RSA - expoente particular. O campo não pode ser lido de volta. |
| n | cadeia de caracteres | Chave RSA - módulo |
| p | cadeia de caracteres | Chave RSA - primeiro prime. O campo não pode ser lido de volta. |
| q | cadeia de caracteres | CHAVE RSA - segundo prime. O campo não pode ser lido de volta. |
| dp | cadeia de caracteres | Chave RSA - primeiro expoente. O campo não pode ser lido de volta. |
| dq | cadeia de caracteres | Chave RSA - segundo expoente. O campo não pode ser lido de volta. |
| qi | cadeia de caracteres | Chave RSA - Coeficiente. O campo não pode ser lido de volta. |
| k | cadeia de caracteres | Chave Simétrica para o tipo de chave de oct. O campo não pode ser lido de volta.   |
| nbf | int | Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.) |
| exp | int | Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.) |



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


