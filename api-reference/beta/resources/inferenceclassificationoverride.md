---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário sobre como as mensagens de entrada de um remetente específico devem sempre ser classificadas como
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548730"
---
# <a name="inferenceclassificationoverride-resource-type"></a>Tipo de recurso inferenceClassificationOverride

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a substituição de um usuário sobre como as mensagens de entrada de um remetente específico devem sempre ser classificadas como em uma [caixa de entrada destaques](manage-focused-inbox.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Update](../api/inferenceclassificationoverride-update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |Altere o campo **ClassifyAs** de uma substituição conforme especificado. |
|[Excluir](../api/inferenceclassificationoverride-delete.md) | None |Exclua uma substituição especificada de acordo com sua ID. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classifyAs|string| Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.|
|id|string| O identificador exclusivo da substituição. Somente leitura.|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassificationoverride.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
