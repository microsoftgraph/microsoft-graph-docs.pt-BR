---
title: Arquivar equipe
description: 'Arquive a equipe especificada. '
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3333f13aad2c6ea11b333acaec0574a2d7dcaf04
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343965"
---
# <a name="archive-team"></a>Arquivar equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Arquive o [team](../resources/team.md) especificado. Quando uma equipe é arquivada, os usuários não podem mais enviar ou curtir mensagens em qualquer canal da equipe, editar o nome, a descrição ou outras configurações da equipe ou, em geral, fazer a maioria das alterações na equipe. As alterações de associação à equipe continuam a ser permitidas.

O arquivamento é uma operação assíncrona. Uma equipe é arquivada assim que a operação assíncrona é concluída com êxito, o que pode ocorrer após uma resposta desta API.

Para arquivar uma equipe, a equipe e [grupo](../resources/group.md) devem ter um proprietário.

Para restaurar uma equipe do estado arquivado, use a API para [desarquivar](team-unarchive.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamSettings.ReadWrite.All, Group.ReadWrite.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | TeamSettings.ReadWrite.Group *, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All** |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent). As permissões marcadas com ** são preteridas e não devem ser usadas.

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

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
Este parâmetro opcional define se as permissões dos membros da equipe devem ser definidas apenas para leitura, no site do SharePoint Online associado à equipe. Essa etapa será ignorada, caso as defina como falsas ou omita o corpo completamente.

## <a name="response"></a>Resposta

Se o arquivamento for iniciado com êxito, esse método retornará um código de resposta `202 Accepted`. A resposta também conterá um cabeçalho `Location`, que contém o local da [teamsAsyncOperation](../resources/teamsasyncoperation.md) criada para lidar com o arquivamento da equipe. Verifique o status da operação de arquivamento fazendo uma solicitação GET para esse local.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/archive-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/archive-team-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.
<!-- {
  "blockType": "response",
  "name": "archive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
