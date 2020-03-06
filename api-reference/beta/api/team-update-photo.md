---
title: Atualizar foto da equipe
description: Atualizar a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 26a0852df065e983de3e926bac06a751e9cc083f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452551"
---
# <a name="update-team-photo"></a>Atualizar foto da equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar a foto (imagem) de uma equipe. A seguir, são apresentados os tamanhos suportados de fotos em HD no Office 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504 e 648x648 pixels. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.

> [!Note]
> Há um limite de 4 MB no tamanho total da solicitação. Isso limita o tamanho da foto a menos de 4 MB.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | image/jpeg. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua os dados binários da foto.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Aqui está um exemplo da solicitação para atualizar uma foto da equipe.

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a>Resposta 

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
