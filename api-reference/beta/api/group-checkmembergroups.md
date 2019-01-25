---
title: 'group: checkMemberGroups'
description: Verifique se a associação na lista especificada dos grupos. Retorna da lista os grupos dos quais
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 838ea805f6732965029690a05e8d3294fdd62c26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514898"
---
# <a name="group-checkmembergroups"></a>group: checkMemberGroups

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verifique se há associação na lista de grupos especificada. Retorna os grupos da lista com os quais o grupo especificado tem uma associação direta ou transitiva.

Você pode verificar até 20 grupos por solicitação. Esta função é compatível com o Office 365 e outros tipos de grupos provisionados no Azure AD. Observe que os Grupos do Office 365 não podem conter grupos, então associações em um Grupo do Office 365 sempre são diretas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | ~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                              |
| Aplicativo                            | ~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All                             |

> **Observação:** esta API atualmente exige o `Directory.Read.All` permissão ou posterior. Usando o `Group.Read.All` permissão retornará um erro. Este é um bug conhecido.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Tipo   | Descrição               |
| :------------ | :----- | :------------------------ |
| Autorização | string | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo   | Descrição           |
| :-------- | :----- | :-------------------- |
| groupIds  | Cadeia de caracteres | Uma matriz de IDs de grupo |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="example"></a>Exemplo

Eis um exemplo de como chamar esta API.

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
