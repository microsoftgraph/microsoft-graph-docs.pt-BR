---
title: tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 14f2121aabaae591187d3033903e569b482b8727
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521240"
---
# <a name="authenticationdetail-resource-type"></a>tipo de recurso authenticationDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes de autenticação para uma entrada de usuário, como informações de autenticação multifator (MFA) e detalhes de PTA/PHS.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo           | Descrição                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | String         | O tipo de método de autenticação usado para executar esta etapa de autenticação. Valores possíveis: `Password` , `SMS` ,,, `Voice` `Authenticator App` `Software OATH token` , `Satisfied by token` .                            |
| authenticationMethodDetail     | String         | Detalhes sobre o método de autenticação usado para executar esta etapa de autenticação. Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para o aplicativo autenticador) e a fonte da senha (por exemplo, nuvem, AD FS, PTA, PHS). |
| authenticationStepDateTime     | DateTimeOffset | Representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.                                           |
| authenticationStepRequirement  | String         | A etapa de autenticação atendida. Por exemplo, autenticação primária ou autenticação multifator.                                                                                                     |
| authenticationStepResultDetail | String         | Detalhes sobre por que a etapa foi bem-sucedida ou falhou. Por exemplo, o usuário é bloqueado, o código de fraude inserido, nenhuma entrada de telefone-tempo limite, telefone inacessível ou declaração no token.                                                     |
| adicionada                      | Boolean        | Indica o status da etapa de autenticação. Valores possíveis: `succeeded` , `failed` .                                                                                                                                 |

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

