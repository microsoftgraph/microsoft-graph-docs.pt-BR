---
title: tipo de recurso agreementFileData
description: Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339136"
---
# <a name="agreementfiledata-resource-type"></a>tipo de recurso agreementFileData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).

## <a name="properties"></a>Propriedades
| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|data|Binária|Dados que representam o documento PDF termos de uso. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
