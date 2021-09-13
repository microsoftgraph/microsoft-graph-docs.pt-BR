---
title: Tipo de recurso UserFlow
description: Representa um fluxo de usuário de identidade incluído em uma jornada de autenticação interna.
ms.localizationpriority: medium
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f2cf68cf056f694c33052e23f9c78db2573c3424
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067357"
---
# <a name="userflow-resource-type"></a>Tipo de recurso UserFlow

Namespace: microsoft.graph

Fluxos de usuário permitem definir políticas predefinidas e configuráveis para entrada, entrada, entrada combinada e entrada, redefinição de senha e atualização de perfil. Esta é uma classe base da que outros fluxos de usuário herdam.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| O identificador do fluxo do usuário. O prefixo **de B2C_1_** é adicionado ao valor que você fornece.|
|userFlowType|userFlowType| Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Único| Esta é a versão do tipo de fluxo do usuário. Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1.1 ou 2.  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
