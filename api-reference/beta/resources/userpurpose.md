---
title: tipo de recurso userpurpose
description: Representa o tipo de destinatário ou de caixa de correio do usuário no Exchange Online.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 83abf3bd19434867bbd162b6260ed5f4445d8ffd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057840"
---
# <a name="userpurpose-resource-type"></a>tipo de recurso userpurpose

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O objetivo da caixa de correio. Usado para diferenciar uma caixa de correio de um único usuário de uma caixa de correio compartilhada e caixa de correio de equipamento no Exchange Online.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|valor|[mailboxRecipientType](#mailboxrecipienttype-values)|Representa o tipo de destinatário ou de caixa de correio do usuário no Exchange Online. Os valores possíveis são: `unknown` , `user` , `linked` , `shared` , `room` , `equipment` e `others` . Consulte a próxima seção para obter mais informações.|

### <a name="mailboxrecipienttype-values"></a>valores de mailboxRecipientType
|Member|Descrição|
|:---------------|:--------|
|desconhecido|Nenhuma informação encontrada sobre a caixa de correio.|
|user|Uma conta de usuário com uma caixa de correio na floresta local.|
|ligado|Uma caixa de correio vinculada a uma conta de usuário em outra floresta.|
|compartilhado|Uma caixa de correio compartilhada por duas ou mais contas de usuário.|
|cômodo|Uma caixa de correio representando uma sala de conferência.|
|equipa|Uma caixa de correio representando uma peça de equipamento.|
|usuários|Caixa de correio encontrada, mas o objetivo do usuário é diferente dos especificados acima.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


