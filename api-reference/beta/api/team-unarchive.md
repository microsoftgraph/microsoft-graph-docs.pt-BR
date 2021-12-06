---
title: Desarquivar equipe
description: Restaure uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, acatando as configurações de locatário e equipe. Teams são arquivados usando a API de arquivo morto.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c68b8fbb97363b598a120d67e9333378c3c8698a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977740"
---
# <a name="unarchive-team"></a>Desarquivar equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Restaurar uma equipe [arquivada.](../resources/team.md) Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, acatando as configurações de locatário e equipe. Teams são arquivados usando a API [de](team-archive.md) arquivo morto.

A desarquivação é uma operação assíncrona. Uma equipe é desarquivada quando a operação assíncrona é concluída com êxito, o que pode ocorrer subsequentemente a uma resposta dessa API.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamSettings.ReadWrite.All, Group.ReadWrite.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | TeamSettings.ReadWrite.Group *, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All** |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](https://aka.ms/teams-rsc). As permissões marcadas com ** são preteridas e não devem ser usadas.

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se a desarquivação for iniciada com êxito, este método retornará um `202 Accepted` código de resposta. A resposta também conterá um header, que contém o local do `Location` [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para lidar com a desarquivação da equipe. Verifique o status da operação de desarquivamento fazendo uma solicitação GET para esse local.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unarchive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unarchive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unarchive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unarchive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unarchive-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.
<!-- {
  "blockType": "response",
  "name": "unarchive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


