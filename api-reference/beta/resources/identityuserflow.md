---
title: Tipo de recurso userflow
description: Os fluxos de usuário de identidade são viagens de autenticação integradas
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d14722844c6449a585ca023df80fccb4e9d7c90b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218454"
---
# <a name="userflow-resource-type"></a>Tipo de recurso userflow

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os fluxos de usuário permitem que você defina políticas configuráveis e predefinidas para entrar, inscrever-se, inscrever-se e entrar, redefinição de senha e atualização de perfil.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/identityuserflow-list.md) | Coleção [Userflow](identityuserflow.md) | Listar transflows. |
| [Create](../api/identityuserflow-post-userflows.md) | [Userflow](identityuserflow.md) | Criar objeto userflow. |
| [Get](../api/identityuserflow-get.md) | [Userflow](identityuserflow.md) | Leia as propriedades e as relações do objeto userflow. |
| [Delete](../api/identityuserflow-delete.md) | None | Exclua o objeto userflow. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|userflowtype|string| Os valores possíveis são: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.|
|userFlowTypeVersion|Único| Esta é a versão do tipo de fluxo do usuário. Cada tipo de fluxo de usuário pode ter diferentes versões possíveis, como 1, 1,1 ou 2.  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
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
