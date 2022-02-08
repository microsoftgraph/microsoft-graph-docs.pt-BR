---
title: Obter foto da equipe
description: Obter a foto (imagem) de uma equipe.
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 01a1641ddb180bf54ce9ded0096240faa5b0535d
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443230"
---
# <a name="get-team-photo"></a>Obter foto da equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha a foto (imagem) de uma equipe ou metadados da foto.

Este método tenta primeiro recuperar a foto especificada do Microsoft 365. Se a foto não estiver disponível no Microsoft 365, ele tentará recuperar a foto do Azure Active Directory.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All** |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All **, Group.ReadWrite.All**, Directory.Read.All **, Directory.ReadWrite.All**  |

> **Observação**: as permissões marcadas com ** têm suporte apenas para compatibilidade com versões anteriores. Recomendamos que você atualize suas soluções para usar permissões diferentes e evite usar essas permissões no futuro. Permissões marcadas com * usem [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

> **Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.

## <a name="http-request"></a>Solicitação HTTP

### <a name="get-the-metadata-of-the-photo"></a>Obter os metadados da foto

Este ponto de extremidade retornará os metadados da foto.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo
```

### <a name="get-the-photo"></a>Obter a foto

Este ponto de extremidade recuperará os dados binários da foto.

<!-- {
  "blockType": "ignored"
}-->

```http
GET /teams/{id}/photo/$value
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo para esta solicitação.

## <a name="response"></a>Resposta

### <a name="response-for-getting-the-metadata-of-a-photo"></a>Resposta para obter os metadados de uma foto

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e metadados sobre a foto.

### <a name="response-for-getting-the-photo"></a>Resposta para obter a foto

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e os dados binários da foto.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-photo-metadata"></a>Exemplo 1: obter os metadados da foto

#### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para obter os metadados da foto da equipe.

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo_metadata"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo
```

#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/teams('ddfcd489-628b-7d04-b48b-20075df800e5')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

### <a name="example-2-get-the-team-photos-binary-data"></a>Exemplo 2: obter os dados binários da foto da equipe

Aqui está um exemplo da solicitação para obter os dados binários da foto da equipe.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "get_team_photo"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/photo/$value
```

#### <a name="response"></a>Resposta

Contém os dados binários da foto solicitada. O código de resposta HTTP é 200.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->