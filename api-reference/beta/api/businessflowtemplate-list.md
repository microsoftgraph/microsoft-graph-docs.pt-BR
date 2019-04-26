---
title: Listar businessFlowTemplates
description: No recurso de revisões do Azure AD Access, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
ms.openlocfilehash: 3d9755a8aefb8c9e9fc4348c2002141805847c5d
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299665"
---
# <a name="list-businessflowtemplates"></a>Listar businessFlowTemplates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [businessFlowTemplate](../resources/businessflowtemplate.md) .
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview. Read. All, AccessReview. ReadWrite. All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | AccessReview. Read. All |

O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo de solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  Criar um novo accessReview. |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
