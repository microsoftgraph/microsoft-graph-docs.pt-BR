---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário de como as mensagens de entrada de um remetente específico sempre devem ser classificadas como
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: abheek-das
ms.openlocfilehash: c0668afef202f646d1d07412077dd15c29747b61
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898578"
---
# <a name="inferenceclassificationoverride-resource-type"></a>Tipo de recurso inferenceClassificationOverride

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a substituição de um usuário de como as mensagens de entrada de um remetente específico sempre devem ser classificadas como em uma Caixa [de Entrada Destaques](manage-focused-inbox.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Altere o campo **ClassifyAs** de uma substituição conforme especificado. |
|[Excluir](../api/inferenceclassificationoverride-delete.md) | Nenhum |Exclua uma substituição especificada de acordo com sua ID. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classifyAs|inferenceClassificationType| Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.|
|id|cadeia de caracteres| O identificador exclusivo da substituição. Somente leitura.|
|senderEmailAddress|[emailAddress](emailaddress.md)|As informações de endereço de email do remetente para quem a substituição é criada.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


