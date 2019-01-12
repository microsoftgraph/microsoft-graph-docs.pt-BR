---
title: Atualizar administrativeunit
description: Atualize as propriedades de um objeto administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cd82035e06fbd6135f4d2f6cbb7f6dfae9576f9a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932011"
---
# <a name="update-administrativeunit"></a>Atualizar administrativeunit

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Atualize as propriedades de um objeto [administrativeUnit](../resources/administrativeunit.md) .
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|string|Descrição para a unidade administrativa.|
|displayName|string|Nome de exibição para a unidade administrativa.|
|visibilidade|string|Visibilidade para a unidade administrativa. Se não estiver definido, então, o padrão é "público". Pode ser definido como "HiddenMembership", que oculta a associação de não-membros.|

Desde que o recurso de **administrativeUnit** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **administrativeUnit** .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
