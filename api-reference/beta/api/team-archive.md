---
title: Equipe de arquivo morto
description: 'Arquive a equipe especificada. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 984fbd7692f28ab2ebf8f3be0411447b51bf2d13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866189"
---
# <a name="archive-team"></a>Equipe de arquivo morto

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Arquive a [equipe](../resources/team.md)de especificado. Quando uma equipe é arquivada, os usuários podem não mais enviar como mensagens em nenhum canal na equipe de, edite o nome da equipe, descrição ou outras configurações ou em geral, verifique a maioria das alterações para a equipe.
As alterações de associação para a equipe continuam a ser permitido.

O arquivamento é uma operação assíncrona. Uma equipe será arquivada depois que a operação assíncrona for concluída com êxito, que podem ocorrer na sequência de resposta dessa API.

Para arquivar equipe, a equipe e o [grupo](../resources/group.md) devem ter um proprietário.

Para restaurar uma equipe de seu estado arquivado, use a API para [unarchive](team-unarchive.md).

## <a name="permissions"></a>Permissions
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
POST /teams/{id}/archive
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Na solicitação, você pode _, opcionalmente,_ inclua o `shouldSetSpoSiteReadOnlyForMembers` parâmetro em um JSON body, da seguinte maneira.
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
Este parâmetro opcional define se deve definir permissões para os membros da equipe como somente leitura no site do Sharepoint Online associado à equipe. Definir como false ou omitindo o corpo todo resultará nesta etapa sendo ignorada.

## <a name="response"></a>Resposta

Se arquivamento for iniciado com êxito, esse método retorna um `202 Accepted` código de resposta. A resposta conterá também um `Location` cabeçalho, que contém o local do [teamsAsyncOperation](../resources/teamsasyncoperation.md) que foi criado para manipular o arquivamento da equipe. Verificar o status da operação de arquivamento, tornando uma solicitação GET para este local.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
O exemplo a seguir é um exemplo de uma solicitação.
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a>Resposta
O exemplo a seguir é um exemplo de uma resposta.
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
