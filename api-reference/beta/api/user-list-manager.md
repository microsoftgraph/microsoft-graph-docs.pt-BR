---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 32784009419596579551430deee3d8953fc1a139
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086764"
---
# <a name="list-manager"></a>Listar gerente

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retorna o usuário ou o contato organizacional atribuído como gerente do usuário. Opcionalmente, você pode expandir a cadeia do gerente para o nó raiz.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP

Obtenha o gerente:
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
Obtenha a cadeia de gerenciamento:
<!-- { "blockType": "ignored" } -->
```http
GET /me?$expand=manager
GET /users?$expand=manager($levels=max)
GET /users/{id | userPrincipalName}/?$expand=manager($levels=max)
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.  

Se sua solicitação incluir o `$expand=manager($levels=max)` parâmetro para obter a cadeia do gerente, você também deverá incluir o seguinte:

- `$count=true` parâmetro de cadeia de caracteres de consulta
- `ConsistencyLevel=eventual` cabeçalho da solicitação

>**Observação:** `max` é o único valor permitido para `$levels` .
> Quando o `$level` parâmetro não é especificado, somente o gerente imediato é retornado.  
> Você pode especificar `$select` dentro `$expand` para selecionar as propriedades do gerente individual: `$expand=manager($levels=max;$select=id,displayName)`

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório.  |
| ConsistencyLevel | eventualmente. Obrigatório quando a solicitação inclui o `$expand=manager($levels=max)` parâmetro. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-manager"></a>Exemplo 1: obter gerente

O exemplo a seguir mostra uma solicitação para obter o gerente.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "<user-id>",
  "displayName": "Sara Davis",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

### <a name="example-2-get-manager-chain-up-to-the-root-level"></a>Exemplo 2: obter cadeia de gerentes até o nível raiz

O exemplo a seguir mostra uma solicitação para obter a cadeia de gerentes até o nível raiz.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_transitive_managers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me?$expand=manager($levels=max;$select=id,displayName)&$select=id,displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. Os gerenciadores transitivos são exibidos hierarquicamente.

>**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "<user1-id>",
    "displayName": "Individual Contributor",
    "manager": {
        "id": "<manager1-id>",
        "displayName": "Manager 1",
        "manager": {
            "id": "<manager2-id>",
            "displayName": "Manager 2",
            "manager": {
                "id": "<manager3-id>",
                "displayName": "Manager 3"
            }
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
