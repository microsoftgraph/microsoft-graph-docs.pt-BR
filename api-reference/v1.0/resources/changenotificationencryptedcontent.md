---
title: Tipo de recurso changeNotificationEncryptedContent
description: Um objeto changeNotificationEncryptedContent representa os dados criptografados anexados a uma notificação de alteração.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 01815c47312b33f9ca3d4dfa3d96df063219628ec28fab7d45066268a39a3f53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246903"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>Tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter mais informações, consulte [Set up change notifications that include resource data (preview)](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | string | Dados criptografados codificados com base64 que produzem um recurso completo respresentado como JSON. Os dados foram criptografados com o fornecido `dataKey` usando um pacote de `AES/CBC/PKCS5PADDING` codificação. |
| dataSignature | string | Hash HMAC-SHA256 codificado com base64 dos dados para fins de validação. |
| dataKey | string | Chave simétrica codificada com base64 gerada pela Microsoft Graph criptografar o valor de dados e gerar a assinatura de dados. Essa chave é criptografada com a chave pública do certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado antes de poder ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | cadeia de caracteres | ID do certificado usado para criptografar `dataKey` o . |
| encryptionCertificateThumbprint | string | Representação hexadecimal da impressão digital do certificado usado para criptografar `dataKey` o . |

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
