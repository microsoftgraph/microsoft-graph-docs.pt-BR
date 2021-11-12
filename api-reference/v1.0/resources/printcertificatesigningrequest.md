---
title: Tipo de recurso printCertificateSigningRequest
description: A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2136ae68a722242e8ad3b7f39743e20d7a54cfe7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944295"
---
# <a name="printcertificatesigningrequest-resource-type"></a>Tipo de recurso printCertificateSigningRequest

Namespace: microsoft.graph

A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|content|Cadeia de caracteres|Uma solicitação de certificado pkcs10 codificada com base64. Somente leitura.|
|transportKey|Cadeia de caracteres|A parte pública codificada com base64 de uma chave assimétrica gerada pelo cliente. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printCertificateSigningRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printCertificateSigningRequest",
  "content": "String",
  "transportKey": "String"
}
```

