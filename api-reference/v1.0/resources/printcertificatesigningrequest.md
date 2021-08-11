---
title: Tipo de recurso printCertificateSigningRequest
description: A solicitação de assinatura de certificado (CSR) a ser usada durante o registro de uma impressora com o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0c86e7a2ecbd164f40dcbb0865954c4549622f16aa1f2b008a392f150b626aa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129972"
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

