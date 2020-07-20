---
title: tipo de recurso printCertificateSigningRequest
description: A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 48b3921dbd9ec616290922fa232bfbbd47da00df
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007141"
---
# <a name="printcertificatesigningrequest-resource-type"></a>tipo de recurso printCertificateSigningRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de impressão universal.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|Uma solicitação de certificado PKCS10 codificada em base64. Somente leitura.|
|transportKey|String|A parte pública codificada em Base64 de uma chave assimétrica gerada pelo cliente. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}-->

```json
{
  "content": "String",
  "transportKey": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printCertificateSigningRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
