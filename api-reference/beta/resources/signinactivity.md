---
title: tipo de recurso signInActivity
description: Fornece a última data de logon de um usuário específico.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8144a681f93df45827c8b304d507eea820adcca2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520594"
---
# <a name="signinactivity-resource-type"></a>tipo de recurso signInActivity

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece a última data de logon de um usuário específico.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|A última data de entrada de um usuário específico. Você pode usar esse campo para calcular a última vez que um usuário entrou no diretório. Este campo pode ser usado para criar relatórios, como usuários inativos. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|lastSignInRequestId|String|ID da solicitação da última entrada realizada por esse usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->