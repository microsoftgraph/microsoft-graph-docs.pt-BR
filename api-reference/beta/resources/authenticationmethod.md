---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fefa2ed8ee17a898b51e7bc21b3e13ec64f68d56
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557833"
---
# <a name="authenticationmethod-resource-type"></a>tipo de recurso authenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um método de autenticação registrado para um usuário. Um [método de autenticação](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema. Alguns exemplos incluem senha, telefone (utilizável via SMS ou chamada de voz), chaves de segurança do FIDO2 e muito mais. No momento, os métodos Password e Phone são implementados.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar authenticationMethods](../api/authentication-list-methods.md) | coleção [AuthenticationMethod](authenticationmethod.md) | Leia as propriedades e os relacionamentos de todos os objetos do usuário **AuthenticationMethod** . |
| [Obter authenticationMethod](../api/authenticationmethod-get.md) | [authenticationMethod](authenticationmethod.md) | Leia as propriedades e os relacionamentos de um objeto **AuthenticationMethod** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador da instância de um método de autenticação registrado para este usuário. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
