---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b052a6034484a5d1d1f8edc8ff9adc3feac52e98
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469133"
---
# <a name="authenticationmethod-resource-type"></a>tipo de recurso authenticationMethod

Namespace: microsoft.graph

Representa um método de autenticação registrado para um usuário. Um [método de autenticação](/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema. Alguns exemplos incluem senha, telefone (usável por SMS ou chamada de voz), chaves de segurança FIDO2 e muito mais.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Autenticação de listaMethods](../api/authentication-list-methods.md) | [Coleção authenticationMethod](authenticationmethod.md) | Leia as propriedades e as relações de todos os objetos **authenticationMethod** de um usuário. |
| [Obter authenticationMethod](../api/authenticationmethod-get.md) | [authenticationMethod](authenticationmethod.md) | Leia as propriedades e as relações de um **objeto authenticationMethod.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| O identificador dessa instância de um método de autenticação registrado nesse usuário. Somente leitura. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationMethod",
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