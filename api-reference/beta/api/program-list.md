---
title: Lista de programas
description: No Windows Azure AD para acessar o recurso de revisões, liste todos os objetos de programa.
localization_priority: Normal
ms.openlocfilehash: 9ea71e5377b7dcfe7ca6de7cfaf221e2c6dfcd98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876290"
---
# <a name="list-programs"></a>Lista de programas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, liste todos os objetos de [programa](../resources/program.md) .
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | `ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.  O usuário conectado também deve ser uma função de diretório que permite a atualização-los para leitura de um programa. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Portador \{token\}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo da solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos do [programa](../resources/program.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista programControls de um programa](program-listcontrols.md) |     coleção [programControl](../resources/programcontrol.md)|    Obter uma coleção dos controles de um programa.|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
