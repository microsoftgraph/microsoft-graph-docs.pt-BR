---
title: Tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de entrada.
ms.localizationpriority: medium
author: rckyplln
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a42697bd49f9f6742c3f6c1e61ace9a8a1362111
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944446"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>Tipo de recurso signInFrequencySessionControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Controle de sessão para impor a frequência de entrada. Herda do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|type          |signinFrequencyType       | Os valores possíveis são: `days`, ou se `null` frequencyInterval for `everyTime` `hours`.|
|valor         |Int32        | O número de `days` ou `hours`.|
|Authenticationtype |signInFrequencyAuthenticationType  | Os valores possíveis são `primaryAndSecondaryAuthentication`, `secondaryAuthentication`. `unknownFutureValue`|
|frequencyInterval  |signInFrequencyInterval  | Os valores possíveis são `timeBased`, `everyTime`. `unknownFutureValue`|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled":true,
  "type": "String",
  "value": 1024,
  "authenticationType": "String",
  "frequencyInterval": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


