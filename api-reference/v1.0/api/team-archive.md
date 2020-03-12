---
title: Arquivar equipe
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d849f4166e0481accb991c6f318e486917e562e3
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2020
ms.locfileid: "42572388"
---
# <a name="archive-team"></a>Arquivar equipe

Namespace: microsoft.graph

Arquive a [equipe ](../resources/team.md) especificada. Quando uma equipe é arquivada, os usuários não podem mais enviar ou curtir mensagens nos canais da equipe, editar o nome, a descrição ou outras configurações da equipe ou, em geral, fazer a maioria das alterações na equipe.
As alterações de associação à equipe continuam a ser permitidas.

O arquivamento é uma operação assíncrona. Uma equipe é arquivada depois que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta dessa API.

Para arquivar uma equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.

Para restaurar uma equipe do estado arquivado, use a API para [desarquivar](team-unarchive.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All    |

> **Observação**: esta API oferece suporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Na solicitação, você pode _opcionalmente_ incluir o parâmetro `shouldSetSpoSiteReadOnlyForMembers` em um corpo JSON, da seguinte maneira.
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
Esse parâmetro opcional define se é necessário definir permissões para membros da equipe como somente leitura no site do SharePoint Online associado à equipe. Essa etapa será ignorada, caso as defina como falsas ou omita o corpo completamente.

>[!IMPORTANT]
>Não há suporte para o parâmetro `shouldSetSpoSiteReadOnlyForMembers` no contexto do aplicativo.

## <a name="response"></a>Resposta

Se o arquivamento for iniciado com êxito, esse método retornará um código de resposta `202 Accepted`. A resposta também conterá um cabeçalho `Location`, que contém o local da [teamsAsyncOperation](../resources/teamsasyncoperation.md) criada para lidar com o arquivamento da equipe. Verifique o status da operação de arquivamento fazendo uma solicitação GET para esse local.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
