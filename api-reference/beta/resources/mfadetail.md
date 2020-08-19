---
title: tipo de recurso mfaDetail
description: 'Indica os detalhes de MFA de uma entrada específica. Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: khotz
ms.openlocfilehash: f58736d890bc530239be413aec9a6920c64856ee
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809359"
---
# <a name="mfadetail-resource-type"></a>tipo de recurso mfaDetail

Namespace: Microsoft. Graph indica os detalhes de MFA de uma entrada específica. Ele inclui o método de autenticação usado para entrar e os detalhes de autenticação (por exemplo: telefone, SMS ou caixa postal)



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
