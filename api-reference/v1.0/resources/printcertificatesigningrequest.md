---
title: Tipo de recurso printCertificateSigningRequest
description: A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4c3eda94bb0809991fe7f711a5290561ef1821d7
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516916"
---
# <a name="printcertificatesigningrequest-resource-type"></a>Tipo de recurso printCertificateSigningRequest

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

