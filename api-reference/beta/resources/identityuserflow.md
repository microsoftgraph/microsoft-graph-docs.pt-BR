---
title: Tipo de recurso UserFlow
description: Fluxos de usuários de identidade são jornadas de autenticação internas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a5cb0bfd61e9b99e9837c36484feefc0ff3a635
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440243"
---
# <a name="userflow-resource-type"></a>Tipo de recurso UserFlow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fluxos de usuário permitem definir políticas predefinidas e configuráveis para entrar, se inscrever, se inscrever e entrar combinados, redefinir senha e atualizar o perfil.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/identityuserflow-list.md) | [Coleção UserFlow](identityuserflow.md) | Listar UserFlows. |
| [Create](../api/identityuserflow-post-userflows.md) | [UserFlow](identityuserflow.md) | Criar objeto UserFlow. |
| [Get](../api/identityuserflow-get.md) | [UserFlow](identityuserflow.md) | Ler propriedades e relações do objeto UserFlow. |
| [Delete](../api/identityuserflow-delete.md) | Nenhum(a) | Excluir objeto UserFlow. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador do fluxo do usuário. O prefixo **de B2C_1_** é adicionado ao valor que você fornece.|
|userFlowType|string| Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
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


