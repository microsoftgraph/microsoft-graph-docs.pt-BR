---
title: Tipo de recurso authenticationDetail
description: Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifatória (MFA) e detalhes de PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b888ec232a95c821ab00f6baa16e787cfbc7dd7f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136623"
---
# <a name="authenticationdetail-resource-type"></a>Tipo de recurso authenticationDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes de autenticação para uma login do usuário, como informações de autenticação multifa factor (MFA) e detalhes de PTA/PHS.

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo           | Descrição                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | String         | O tipo de método de autenticação usado para executar essa etapa de autenticação. Valores possíveis: `Password` , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .                            |
| authenticationMethodDetail     | String         | Detalhes sobre o método de autenticação usado para executar essa etapa de autenticação. Por exemplo, número de telefone (para SMS e voz), nome do dispositivo (para aplicativo Autenticador) e fonte de senha (por exemplo, nuvem, AD FS, PTA, PHS). |
| authenticationStepDateTime     | DateTimeOffset | Representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.                                           |
| authenticationStepRequirement  | String         | A etapa de autenticação que isso atendia. Por exemplo, autenticação principal ou autenticação multifa factor.                                                                                                     |
| authenticationStepResultDetail | String         | Detalhes sobre por que a etapa foi bem-sucedida ou falhou. Por exemplo, o usuário está bloqueado, o código de fraude inserido, nenhuma entrada de telefone - tempo exemplado, telefone inacessível ou declaração em token.                                                     |
| succeeded                      | Boolean        | Indica o status da etapa de autenticação. Valores possíveis: `succeeded` , `failed` .                                                                                                                                 |

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

