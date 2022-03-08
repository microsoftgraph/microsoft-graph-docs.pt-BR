---
title: Tipo de recurso changeNotificationEncryptedContent
description: Um objeto changeNotificationEncryptedContent representa os dados criptografados anexados a uma notificação de alteração.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: eab67f8a390b6522f963b004670e31e256078353
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334104"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>Tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter detalhes, consulte [Set up change notifications that include resource data (preview)](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | cadeia de caracteres | Dados criptografados codificados com base64 que produzem um recurso completo respresentado como JSON. Os dados foram criptografados com o fornecido usando `dataKey` um pacote `AES/CBC/PKCS5PADDING` de codificação. |
| dataSignature | cadeia de caracteres | Hash HMAC-SHA256 codificado com base64 dos dados para fins de validação. |
| dataKey | cadeia de caracteres | Chave simétrica codificada com base64 gerada pela Microsoft Graph criptografar o valor de dados e gerar a assinatura de dados. Essa chave é criptografada com a chave pública do certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado antes de poder ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding`. |
| encryptionCertificateId | cadeia de caracteres | ID do certificado usado para criptografar o `dataKey`. |
| encryptionCertificateThumbprint | cadeia de caracteres | Representação hexadecimal da impressão digital do certificado usado para criptografar o `dataKey`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationEncryptedContent",
  "data": "String",
  "dataSignature": "String",
  "dataKey": "String",
  "encryptionCertificateId": "String",
  "encryptionCertificateThumbprint": "String"
}
```

<!-- uuid: 564a955a-4837-424d-b7b8-3c6c33d5176d
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "changeNotificationEncryptedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


