---
title: Tipo de recurso persistentBrowserSessionControl
description: Controle de sessão para definir se os cookies serão persistentes ou não.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 52c4efd5d7a3bfb87c34ab07ba84349c6d392af3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117820"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a>Tipo de recurso persistentBrowserSessionControl

Namespace: microsoft.graph

Controle de sessão para definir se os cookies serão persistentes ou não. Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|mode|persistentBrowserSessionMode| Os valores possíveis são: `always`, `never`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

