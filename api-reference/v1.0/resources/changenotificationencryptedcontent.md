---
title: Tipo de recurso changeNotificationEncryptedContent
description: Um objeto changeNotificationEncryptedContent representa os dados criptografados anexados a uma notificação de alteração.
ms.localizationpriority: medium
author: baywet
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: c1ee1628796a8c9e3d527a965363f59b79d11242
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334384"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>Tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter mais informações, consulte [Set up change notifications that include resource data (preview)](/graph/webhooks-with-resource-data.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | string | Dados criptografados codificados com base64 que produzem um recurso completo respresentado como JSON. Os dados foram criptografados com o fornecido usando `dataKey` um pacote `AES/CBC/PKCS5PADDING` de codificação. |
| dataSignature | string | Hash HMAC-SHA256 codificado com base64 dos dados para fins de validação. |
| dataKey | string | Chave simétrica codificada com base64 gerada pela Microsoft Graph criptografar o valor de dados e gerar a assinatura de dados. Essa chave é criptografada com a chave pública do certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado antes de poder ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding`. |
| encryptionCertificateId | cadeia de caracteres | ID do certificado usado para criptografar o `dataKey`. |
| encryptionCertificateThumbprint | string | Representação hexadecimal da impressão digital do certificado usado para criptografar o `dataKey`. |

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
