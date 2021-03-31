---
title: Tipo de recurso changeNotificationEncryptedContent
description: Um objeto changeNotificationEncryptedContent representa os dados criptografados anexados a uma notificação de alteração.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 193f5eb36f19de1b3fd44112bf6bc56b19746911
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468734"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>Tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter detalhes, [consulte Set up change notifications that include resource data (preview)](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | cadeia de caracteres | Dados criptografados codificados com base64 que produzem um recurso completo respresentado como JSON. Os dados foram criptografados com o fornecido `dataKey` usando um pacote de `AES/CBC/PKCS5PADDING` codificação. |
| dataSignature | cadeia de caracteres | Hash HMAC-SHA256 codificado com base64 dos dados para fins de validação. |
| dataKey | cadeia de caracteres | Chave simétrica codificada com base64 gerada pelo Microsoft Graph para criptografar o valor dos dados e gerar a assinatura de dados. Essa chave é criptografada com a chave pública do certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado antes de poder ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | cadeia de caracteres | ID do certificado usado para criptografar `dataKey` o . |
| encryptionCertificateThumbprint | cadeia de caracteres | Representação hexadecimal da impressão digital do certificado usado para criptografar `dataKey` o . |

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

<!-- uuid: 564a955a-4837-424d-b7b8-3c6c33d5176d
2020-05-25 14:57:30 UTC -->
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


