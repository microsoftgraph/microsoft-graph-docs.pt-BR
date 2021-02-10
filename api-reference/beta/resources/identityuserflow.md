---
title: Tipo de recurso UserFlow
description: Os fluxos de identidade do usuário são jornadas de autenticação internas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa6829d346fc1e2520fb5eab28f5ce5fd9c72ae4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176966"
---
# <a name="userflow-resource-type"></a>Tipo de recurso UserFlow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os Fluxos de Usuário permitem definir políticas predefinidas e configuráveis para entrar, inscrever-se, se inscrever e entrar combinados, redefinição de senha e atualização de perfil.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/identityuserflow-list.md) | [Coleção UserFlow](identityuserflow.md) | Listar UserFlows. |
| [Criar](../api/identityuserflow-post-userflows.md) | [UserFlow](identityuserflow.md) | Crie um objeto UserFlow. |
| [Get](../api/identityuserflow-get.md) | [UserFlow](identityuserflow.md) | Leia as propriedades e os relacionamentos do objeto UserFlow. |
| [Delete](../api/identityuserflow-delete.md) | Nenhum | Exclua o objeto UserFlow. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| O identificador do fluxo do usuário. O prefixo **B2C_1_** é adicionado ao valor que você fornece.|
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


