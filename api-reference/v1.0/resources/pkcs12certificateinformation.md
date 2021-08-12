---
title: Tipo de recurso pkcs12CertificateInformation
description: Representa as informações públicas de um certificado de cliente Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6b0fe760be0fb67a92d99bbb53125cb79ad9204daf7484f5b8f2292f70a7fea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235363"
---
# <a name="pkcs12certificateinformation-resource-type"></a>Tipo de recurso pkcs12CertificateInformation

Namespace: microsoft.graph

Representa as informações públicas de um certificado Pkcs12.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isActive|Booliano|  Representa se o certificado é o certificado ativo a ser usado para chamar o conector de API. O certificado ativo é o certificado carregado mais recentemente que ainda não expirou, mas cujo tempo de notBefore não está no passado.|
|thumbprint|Cadeia de caracteres| A impressão digital do certificado. |
|notAfter|Inteiro| O certificado expirou. Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)|
|notBefore|Inteiro| O tempo de emissão do certificado (não antes). Esse valor é um NumericDate conforme definido na RFC 7519 (um valor numérico JSON que representa o número de segundos de 1970-01-01T00:00:00Z UTC até a data/hora UTC especificada, ignorando segundos bissexto.)|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
