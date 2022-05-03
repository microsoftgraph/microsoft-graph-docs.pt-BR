---
title: Tipo de recurso printCertificateSigningRequest
description: A CSR (solicitação de assinatura de certificado) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 466782f93ef6de645f8a1b90085e7a96538f1cba
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176913"
---
# <a name="printcertificatesigningrequest-resource-type"></a>Tipo de recurso printCertificateSigningRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A CSR (solicitação de assinatura de certificado) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|content|Cadeia de caracteres|Uma solicitação de certificado pkcs10 codificada em base64. Somente leitura.|
|transportKey|Cadeia de Caracteres|A parte pública codificada em base64 de uma chave assimétrica gerada pelo cliente. Somente leitura.|

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


