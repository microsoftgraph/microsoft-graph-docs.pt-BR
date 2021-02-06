---
title: Tipo de recurso trustFrameworkKey
description: Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na RFC 7517 Seção 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3de9ce67298f31b3c40682040da69f5c2f6ba007
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135853"
---
# <a name="trustframeworkkey-resource-type"></a>Tipo de recurso trustFrameworkKey

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um JWK (chave Web JSON). TrustFrameworkKey é uma estrutura de dados JSON que representa uma chave criptográfica. A estrutura desse recurso segue o formato definido na [RFC 7517 Seção 4](https://tools.ietf.org/html/rfc7517#section-4).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| olh | string | O identificador exclusivo da chave.   |
| kty | string | O parâmetro "kty" (tipo de chave) identifica a família de algoritmos criptográficos usada com a chave, os valores válidos são rsa, oct. |
| use | string | O parâmetro "use" (uso de chave pública) identifica o uso pretendido da chave pública.  O parâmetro "use" é empregado para indicar se uma chave pública é usada para criptografar dados ou verificar a assinatura nos dados. Os valores possíveis são 1. "sig" (assinatura) 2.  "enc" (criptografia)   |
| x5c | coleção de cadeias de caracteres | O parâmetro "x5c" (cadeia de certificados X.509) contém uma cadeia de um ou mais certificados PKIX [RFC 5280.](https://tools.ietf.org/html/rfc5280) |
| x5t | string | O parâmetro "x5t" (certificado X.509 SHA-1 thumbprint) é uma impressão digital SHA-1 codificada em base64url (ou seja, digest) da codificação DER de um certificado X.509 [RFC 5280](https://tools.ietf.org/html/rfc5280). |
| e | string | Chave RSA - expoente público |
| d| string | Chave RSA - expoente privado. O campo não pode ser lido novamente. |
| n | string | Chave RSA - módulo |
| p | string | Chave RSA - primeiro prime. O campo não pode ser lido novamente. |
| q | cadeia de caracteres | Chave RSA - segundo prime. O campo não pode ser lido novamente. |
| dp | string | Chave RSA - primeiro expoente. O campo não pode ser lido novamente. |
| dq | string | Chave RSA - segundo expoente. O campo não pode ser lido novamente. |
| 2013 | string | Chave RSA - Coeficiente. O campo não pode ser lido novamente. |
| k | string | Chave simétrica para o tipo de chave de oct. O campo não pode ser lido novamente.   |
| nbf | int | Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.) |
| exp | int | Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON representando o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.) |



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


