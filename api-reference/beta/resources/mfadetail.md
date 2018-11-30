---
title: tipo de recurso de mfaDetail
description: 'Indica os detalhes MFA para uma entrada específica. Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036417"
---
# <a name="mfadetail-resource-type"></a>tipo de recurso de mfaDetail
Indica os detalhes MFA para uma entrada específica. Inclui o método de autenticação usado para fazer o login, bem como detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|authDetail|String|Indica o detalhe de autenticação MFA da atividade de entrada correspondentes quando o MFA necessário é "Yes".|
|authMethod|String|Indica os métodos de autenticação MFA (SMS, telefone, autenticador App são alguns do valor) para a atividade de entrada correspondente quando o campo MFA necessário é "Yes".|

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