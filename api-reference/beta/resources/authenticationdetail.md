---
title: Tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 134c3e502fa39fea626216315056adfeef5aef13
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720333"
---
# <a name="authenticationdetail-resource-type"></a>Tipo de recurso authenticationDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes PTA/PHS.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo           | Descrição                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | Cadeia de caracteres         | O tipo de método de autenticação usado para executar esta etapa de autenticação. Valores possíveis: `Password` , , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .                            |
| authenticationMethodDetail     | Cadeia de caracteres         | Detalhes sobre o método de autenticação usado para executar essa etapa de autenticação. Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para aplicativo Autenticador) e fonte de senha (por exemplo, nuvem, AD FS, PTA, PHS). |
| authenticationStepDateTime     | DateTimeOffset | Representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.                                           |
| authenticationStepRequirement  | Cadeia de caracteres         | A etapa de autenticação que isso satisfez. Por exemplo, autenticação primária ou autenticação multifa factor.                                                                                                     |
| authenticationStepResultDetail | Cadeia de caracteres         | Detalhes sobre por que a etapa foi bem-sucedida ou falhou. Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone - tempo de tempo, telefone inacessível ou declaração em token.                                                     |
| bem-sucedido                      | Booliano        | Indica o status da etapa de autenticação. Valores possíveis: `succeeded` , `failed` .                                                                                                                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

