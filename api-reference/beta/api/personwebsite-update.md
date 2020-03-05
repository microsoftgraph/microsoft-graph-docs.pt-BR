---
title: Atualizar personWebsite
description: Atualiza as propriedades de um objeto personWebsite no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b93d1ea6fa1449bf6491d3ed574e709ff2c883c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455862"
---
# <a name="update-personwebsite"></a>Atualizar personwebsite

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades do objeto [personWebsite](../resources/personwebsite.md) no [perfil](../resources/profile.md)de um usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User. ReadWrite, User. ReadWrite. All          |
| Delegado (conta pessoal da Microsoft) | User. ReadWrite, User. ReadWrite. All          |
| Aplicativo                            | User.ReadWrite.All                          |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           |Descrição                  |
|:---------------|:----------------------------|
| Autorização  | {token} de portador. Obrigatório.   |
| Content-Type   | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo            | Descrição                                                                         |
|:-------------|:----------------|:------------------------------------------------------------------------------------|
|categories    |String collection| Contém categorias que um usuário associou ao site (por exemplo: pessoal, receitas)  |
|description   |String           | Contém uma descrição do site.                                              |
|displayName   |Cadeia de caracteres           | Contém um nome amigável para o site.                                           |
|webUrl        |String           | Contém um link para o próprio site.                                              |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [personWebsite](../resources/personwebsite.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/user/profile/websites/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personwebsite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->