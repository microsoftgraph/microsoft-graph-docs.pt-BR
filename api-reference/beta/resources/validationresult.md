---
title: Tipo de recurso validationResult
description: Expõe as propriedades que especificam as regras nas quais a senha de um usuário foi validada e os resultados da validação.
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 2e77770749ba06fed83e2855ff465922420da988
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689206"
---
# <a name="validationresult-resource-type"></a>Tipo de recurso validationResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Expõe as propriedades que especificam as regras nas quais a senha de um usuário foi validada e os resultados da validação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mensagem|String| A cadeia de caracteres que contém o motivo pelo qual a regra passou ou não. Somente leitura. Não anulável.|
|ruleName|Cadeia de caracteres| A cadeia de caracteres que contém o nome da regra de validação de senha em que a ação foi validada. Somente leitura. Não anulável.|
|validationPassed|Booliano| Se a senha passou ou falhou na regra de validação. Somente leitura. Não anulável.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.validationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.validationResult",
  "ruleName": "String",
  "validationPassed": "Boolean",
  "message": "String"
}
```

