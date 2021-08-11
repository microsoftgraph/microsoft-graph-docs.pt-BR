---
title: Tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4aa2ecb3c3d16ad942458da190247f1d6f6cb87babc926c97c95605d21d5418d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235678"
---
# <a name="certificateauthority-resource-type"></a>Tipo de recurso certificateAuthority

Namespace: microsoft.graph

Representa uma autoridade de certificação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|certificado|Binário|Obrigatório. A cadeia de caracteres codificada base64 que representa o certificado público.|
|certificateRevocationListUrl|String|A URL da lista de revogação de certificados.|
|deltaCertificateRevocationListUrl|Cadeia de caracteres|A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revogação de certificado completo foi criada.|
|isRootAuthority|Booliano|Obrigatório. **true** se o certificado confiável for uma autoridade raiz, **false** se o certificado confiável for uma autoridade intermediária.|
|emissor|String|O emissor do certificado, calculado a partir do valor **do** certificado. Somente leitura. |
|issuerSki|Cadeia de caracteres|O identificador da chave de assunto do certificado, calculado a partir do **valor do** certificado. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
