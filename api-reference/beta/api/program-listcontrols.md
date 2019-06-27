---
title: Listar programControls de um programa
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl vinculados a um programa específico.
localization_priority: Normal
ms.openlocfilehash: 0c148cea7f15fd52728b51d37ae1bb9cae16edbd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268002"
---
# <a name="list-programcontrols-of-a-program"></a>Listar programControls de um programa

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) vinculados a um programa específico.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | ProgramControl. Read. All, ProgramControl. ReadWrite. All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | ProgramControl. Read. All, ProgramControl. ReadWrite. All  |

 O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo de solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programControl_from_program-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programControl_from_program-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_programControl_from_program-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/program-listcontrols.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
