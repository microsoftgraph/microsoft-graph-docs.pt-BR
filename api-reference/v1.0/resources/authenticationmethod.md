---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 082ae6530ad429df632ba851483a2d3edf16c49778ac22effaaaf01f897be6a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160075"
---
# <a name="authenticationmethod-resource-type"></a>tipo de recurso authenticationMethod

Namespace: microsoft.graph

Representa um método de autenticação registrado para um usuário. Um [método de autenticação](/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema. Alguns exemplos incluem senha, telefone (usável por SMS ou chamada de voz), chaves de segurança FIDO2 e muito mais.

> [!IMPORTANT]
> Listar os métodos de autenticação dos usuários retorna apenas os métodos suportados nesta versão da API. Consulte [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Autenticação de listaMethods](../api/authentication-list-methods.md) | [Coleção authenticationMethod](authenticationmethod.md) | Leia as propriedades e as relações de todos os objetos **authenticationMethod** de um usuário. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| O identificador dessa instância de um método de autenticação registrado nesse usuário. Somente leitura. |

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