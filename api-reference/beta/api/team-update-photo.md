---
title: Atualizar foto da equipe
description: Atualizar a foto (imagem) de uma equipe.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22fdca19b657bdf439f356fb61e4f805f45b4f4b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896123"
---
# <a name="update-team-photo"></a>Atualizar foto da equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar a foto (imagem) de uma equipe. Estes são os tamanhos de fotos de HD compatíveis no Microsoft 365:48x48, 64x64, 96x96, 120x120, 240x240, 360X360, 432x432, 504x504 e 648x648 pixels. As fotos podem ser de todos os tamanhos, desde que estejam armazenadas no Azure Active Directory.

> [!Note]
> Há um limite de 4 MB no tamanho total da solicitação. Isso limita o tamanho da foto a menos de 4 MB.

## <a name="permissions"></a>Permissões

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamSettings. Edit. Group *, TeamSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |

> **Observação**: as permissões marcadas com * usam o [consentimento específico do recurso](https://aka.ms/teams-rsc).

> **Observação**: esta API oferece transporte a permissões de administrador. Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | Bearer {token}. Required.  |
| Content-type | image/jpeg. Required.  |

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
