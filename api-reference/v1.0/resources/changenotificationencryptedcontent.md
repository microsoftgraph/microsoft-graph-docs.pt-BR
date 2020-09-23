---
title: tipo de recurso changeNotificationEncryptedContent
description: Um objeto changeNotificationEncryptedContent representa os dados criptografados anexados a uma notificação de alteração.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f86dc032e3f9e14790358a03e8026f1932ae9431
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193628"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter mais informações, consulte [configurar notificações de alteração que incluem dados de recurso (visualização)](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | string | Dados criptografados codificados em base64 que produzem um respresented de recurso completo como JSON. Os dados foram criptografados com o fornecido `dataKey` usando um `AES/CBC/PKCS5PADDING` pacote de codificação. |
| DataSignature | string | Hash HMAC-SHA256 codificado em base64 dos dados para fins de validação. |
| DataKeyNames | string | Chave simétrica codificada em base64 gerada pelo Microsoft Graph para criptografar o valor dos dados e gerar a assinatura dos dados. Essa chave é criptografada com a chave pública de certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado para que possa ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | string | ID do certificado usado para criptografar o `dataKey` . |
| encryptionCertificateThumbprint | string | Representação hexadecimal da impressão digital do certificado usado para criptografar o `dataKey` . |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->

```json
{
  "data": "{encrypted data that produces a full resource}",
  "dataSignature": "<HMAC-SHA256 hash>",
  "dataKey": "{encrypted symmetric key from Microsoft Graph}",
  "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
  "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
}
```

<!-- uuid: 6bb14c3d-16ef-4ea3-8dc7-c88b9190081c
2020-08-05 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedConent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
