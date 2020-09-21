---
title: tipo de recurso printCertificateSigningRequest
description: A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 786c5224826040e685f27a131cb81f07e1eebd7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084006"
---
# <a name="printcertificatesigningrequest-resource-type"></a>tipo de recurso printCertificateSigningRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de impressão universal.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|Uma solicitação de certificado PKCS10 codificada em base64. Somente leitura.|
|transportKey|Cadeia de caracteres|A parte pública codificada em Base64 de uma chave assimétrica gerada pelo cliente. Somente leitura.|

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


