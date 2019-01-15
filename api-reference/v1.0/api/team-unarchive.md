---
title: Equipe de unarchive
description: Restaure uma equipe arquivada. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe. As equipes são arquivadas usando a API de arquivamento.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b015be832093b0e68f304600afbc52421f654857
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016706"
---
# <a name="unarchive-team"></a>Equipe de unarchive



Restaure uma [equipe](../resources/team.md)de arquivados. Isso restaura a capacidade dos usuários de enviar mensagens e editar a equipe, aceitar pelas configurações de locatário e equipe. As equipes são arquivadas usando o [arquivo morto](team-archive.md) API.

Unarchiving é uma operação assíncrona. Uma equipe é não arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All    |

> **Observação**: Esta API oferece suporte a permissões de administrador. Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.

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

Se unarchiving for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta. A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular unarchiving da equipe. Verificar o status da operação unarchiving fazendo uma solicitação GET para este local.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
O exemplo a seguir é um exemplo de uma solicitação.
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```

#### <a name="response"></a>Resposta
O exemplo a seguir é um exemplo de uma resposta.
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
