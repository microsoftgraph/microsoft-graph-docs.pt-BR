---
title: Obter operação de autenticação
description: Recupere as propriedades e os relacionamentos de um objeto Operation.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8340fe68f865fa9acfba0cbb05537422e2cfacf9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805772"
---
# <a name="get-authentication-operation"></a>Obter operação de autenticação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e os relacionamentos de um objeto [Operation](../resources/operation.md) . Atualmente, essas operações são geradas iniciando uma redefinição de senha usando o método [Reset password](passwordauthenticationmethod-resetpassword.md) . Um objeto Operation informa ao chamador sobre o estado atual da operação de redefinição de senha. Os Estados possíveis incluem:

* NotStarted
* Em execução
* Succeeded
* Falhou

`Succeeded`e `Failed` são Estados de terminal.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões que atuam em si (de menos para mais privilégios) | Permissões que atuam em outros (de menos para mais privilégios)|
|:---------------------------------------|:-------------------------|:-----------------|
| Delegado (conta corporativa ou de estudante)     | UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All | UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. | Sem suporte. |
| Aplicativo                            | Sem suporte. | Sem suporte. |

Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Administrador global
* Leitor global
* Administrador de autenticação privilegiada
* Administrador de autenticação

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/authentication/operations/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [Operation](../resources/operation.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_operation"
}-->

```msgraph-interactive
GET /users/{id}/authentication/operations/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-operation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-operation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-operation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.operation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "status": "running",
  "createdDateTime": "2020-03-19T12-01-03.45Z",
  "lastActionDateTime": "2020-03-19T12-01-04.23Z",
  "id": "2d497bb-57bd-47a6-8749-5ccd0869f2bd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get operation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
