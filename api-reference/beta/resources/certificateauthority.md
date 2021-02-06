---
title: Tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64461015136129de452227cb0a8de5c7180cfb32
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135091"
---
# <a name="certificateauthority-resource-type"></a>Tipo de recurso certificateAuthority

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma autoridade de certificação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|certificado|Binário|Obrigatório. A cadeia de caracteres codificada em base64 que representa o certificado público.|
|certificateRevocationListUrl|String|A URL da lista de certificados revogados.|
|deltaCertificateRevocationListUrl|String|A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de certificados revogados completos foi criada.|
|isRootAuthority|Boolean|Obrigatório. **true** se o certificado confiável for uma autoridade raiz, **false** se o certificado confiável for uma autoridade intermediária.|
|emissor|String|O emissor do certificado, calculado a partir do valor **do** certificado. Somente leitura. |
|issuerSki|String|O identificador da chave de assunto do certificado, calculado a partir do valor **do** certificado. Somente leitura.|

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

