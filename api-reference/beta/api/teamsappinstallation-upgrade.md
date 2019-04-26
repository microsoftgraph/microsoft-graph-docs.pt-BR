---
title: Atualizar um aplicativo em uma equipe
description: Atualiza uma instalação de aplicativo em uma equipe
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 569fb5b0f8f117ebfa8496fd5f9b2ba023a113d9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335270"
---
# <a name="upgrade-an-app-in-a-team"></a>Atualizar um aplicativo em uma equipe

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza uma [instalação de aplicativo](../resources/teamsappinstallation.md) em uma [equipe](../resources/team.md) para a versão mais recente do aplicativo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
