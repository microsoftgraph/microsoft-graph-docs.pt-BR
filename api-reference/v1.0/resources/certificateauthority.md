---
title: tipo de recurso certificateAuthority
description: Representa uma autoridade de certificação.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50555ff47d81d96def360fe55fe8684f6ff07994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531949"
---
# <a name="certificateauthority-resource-type"></a>tipo de recurso certificateAuthority

Namespace: microsoft.graph

Representa uma autoridade de certificação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|certificado|Binário|Obrigatório. A cadeia de caracteres codificada em base64 que representa o certificado público.|
|certificateRevocationListUrl|String|A URL da lista de certificados revogados.|
|deltaCertificateRevocationListUrl|String|A URL contém a lista de todos os certificados revogados desde a última vez que uma lista de revocaton de certificados completo foi criada.|
|isRootAuthority|Booliano|Obrigatório. **true** se o certificado confiável é uma autoridade raiz, **false** se o certificado confiável é uma autoridade intermediária.|
|emissor|String|O emissor do certificado, calculado com base no valor do **certificado** . Somente leitura. |
|issuerSki|String|O identificador de chave de entidade do certificado, calculado com base no valor do **certificado** . Somente leitura.|

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