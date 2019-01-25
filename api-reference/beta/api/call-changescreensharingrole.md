---
title: 'chamar: changeScreenSharingRole'
description: Iniciar e interromper o compartilhamento de tela na chamada. Essa API é usada para permitir que aplicativos compartilhar o conteúdo de tela com os participantes de uma chamada ou reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f0bdd9a4c8e900d9a1ec5f7801fa959ebdaae1e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514730"
---
# <a name="call-changescreensharingrole"></a>chamar: changeScreenSharingRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Iniciar e interromper o compartilhamento de tela na chamada. Essa API é usada para permitir que aplicativos compartilhar o conteúdo de tela com os participantes de uma chamada ou reunião.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não suportado                               |
| Delegado (conta pessoal da Microsoft) | Não suportado                               |
| Aplicativo                            | Calls.AccessMedia.All                       |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro      | Tipo    |Descrição|
|:---------------|:--------|:----------|
|role|String|Os valores possíveis são: 'Visualizador', 'Compartilhador'|

## <a name="response"></a>Resposta
Retorna `202 Accepted` código de resposta.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
