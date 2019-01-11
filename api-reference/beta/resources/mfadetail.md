---
title: tipo de recurso de mfaDetail
description: 'Indica os detalhes MFA para uma entrada específica. Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883738"
---
# <a name="mfadetail-resource-type"></a>tipo de recurso de mfaDetail
Indica os detalhes MFA para uma entrada específica. Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|authDetail|Cadeia de caracteres|Indica o detalhe de autenticação MFA da atividade de entrada correspondentes quando o MFA necessário é "Yes".|
|authMethod|Cadeia de caracteres|Indica os métodos de autenticação MFA (SMS, telefone, autenticador App são alguns do valor) para a atividade de entrada correspondente quando o campo MFA necessário é "Yes".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
