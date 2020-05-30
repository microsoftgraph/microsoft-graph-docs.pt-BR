---
title: tipo de recurso changeNotificationEncryptedContent
description: Uma assinatura com dados de recurso permite que um aplicativo cliente receba notificações de alteração com alterações nos dados no Microsoft Graph. O conteúdo criptografado notificação de alteração representa os dados criptografados anexados à notificação.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1b89fcf99ed4a724bb86413d6ef369b121e28cd3
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430574"
---
# <a name="changenotificationencryptedcontent-resource-type"></a>tipo de recurso changeNotificationEncryptedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os dados criptografados anexados a uma notificação de alteração.

Para obter detalhes, consulte [set up Change Notifications que incluem dados de recurso (visualização)](/graph/webhooks-with-resource-data.md).

## <a name="methods"></a>Methods

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| data | string | Dados criptografados codificados em base64 que produzem um respresented de recurso completo como JSON. Os dados foram criptografados com o fornecido `dataKey` usando um `AES/CBC/PKCS5PADDING` pacote de codificação. |
| DataSignature | string | Hash HMAC-SHA256 codificado em base64 dos dados para fins de validação. |
| DataKeyNames | string | Chave simétrica codificada em base64 gerada pelo Microsoft Graph para criptografar o valor dos dados e gerar a assinatura dos dados. Essa chave é criptografada com a chave pública de certificado fornecida durante a assinatura. Ele deve ser descriptografado com a chave privada do certificado para que possa ser usado para descriptografar os dados ou verificar a assinatura. Essa chave foi criptografada com o seguinte pacote de codificação: `RSA/ECB/OAEPWithSHA1AndMGF1Padding` . |
| encryptionCertificateId | string | ID do certificado usado para criptografar o `dataKey` . |
| encryptionCertificateThumbprint | string | Representação hexadecimal da impressão digital do certificado usado para criptografar o `dataKey` . |

## <a name="relationships"></a>Relações

Nenhum

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
