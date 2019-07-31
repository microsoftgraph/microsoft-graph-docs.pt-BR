---
title: tipo de recurso mfaDetail
description: 'Indica os detalhes de MFA de uma entrada específica. Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f38fae4d0360386592f956bee05d55738ad6910
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009661"
---
# <a name="mfadetail-resource-type"></a>tipo de recurso mfaDetail
Indica os detalhes de MFA de uma entrada específica. Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) 



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|authDetail|String|Indica o detalhe de autenticação da MFA para a atividade de entrada correspondente quando a MFA necessária for "Sim".|
|authMethod|String|Indica os métodos de autenticação da MFA (SMS, Phone, o aplicativo autenticador são alguns dos valores) para a atividade de entrada correspondente quando o campo obrigatório do MFA é "Yes".|

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
