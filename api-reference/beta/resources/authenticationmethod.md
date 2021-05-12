---
title: tipo de recurso authenticationMethod
description: Representa um método de autenticação registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9ab808934491793b796be1c66fc87051ed6e9b29
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335622"
---
# <a name="authenticationmethod-resource-type"></a>tipo de recurso authenticationMethod

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um método de autenticação registrado para um usuário. Um [método de autenticação](/azure/active-directory/authentication/concept-authentication-methods) é algo usado por um usuário para autenticar ou provar sua identidade para o sistema. Alguns exemplos incluem senha, telefone (que pode ser SMS ou chamada de voz), teclas de segurança FIDO2 e muito mais.

> [!IMPORTANT]
> Listar os métodos de autenticação dos usuários retorna apenas os métodos suportados nesta versão da API. Consulte [Azure AD authentication methods API overview](authenticationmethods-overview.md) for a list of currently supported methods.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Autenticação de listaMethods](../api/authentication-list-methods.md) | [Coleção authenticationMethod](authenticationmethod.md) | Leia as propriedades e as relações de todos os objetos **authenticationMethod** de um usuário. |

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