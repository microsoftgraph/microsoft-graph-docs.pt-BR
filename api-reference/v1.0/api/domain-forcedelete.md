---
title: Forçar a exclusão de domínio
description: Exclui um domínio usando uma operação de longa execução assíncrona.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6ba7dd7cf8a29ddfa008931ee8f210caf6bcc872
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973925"
---
# <a name="force-domain-deletion"></a>Forçar a exclusão de domínio

Namespace: microsoft.graph

Exclui um domínio usando uma operação de longa execução assíncrona.

Antes de chamar [forceDelete](domain-forcedelete.md), você deve atualizar ou remover quaisquer referências **Exchange** como o serviço de provisionamento.

As seguintes ações são executadas como parte desta operação:

* Atualiza as propriedades , e de com referências ao domínio excluído para usar o `userPrincipalName` `mail` domínio onmicrosoft.com `proxyAddresses` `users` inicial.

* Atualiza a propriedade de com referências ao domínio excluído para usar o `mail` `groups` domínio onmicrosoft.com inicial.

* Atualiza a propriedade de com referências ao domínio excluído para usar o `identifierUris` `applications` domínio onmicrosoft.com inicial.

* Se o número de objetos a serem renomeados for maior do que 1000, um erro será retornado.

* Se um dos a `applications` ser renomeado for um aplicativo de vários locatários, um erro será retornado.

Após a conclusão da exclusão de domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404. Para verificar a exclusão de um domínio, você pode executar uma [operação obter domínio.](domain-get.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Domain.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Domain.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo | Descrição |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Opção para desabilitar contas de usuário renomeadas. Se uma conta de usuário estiver desabilitada, o usuário não poderá entrar. Se definido como **true,** `users` a atualização como parte dessa operação será desabilitada.  O valor padrão é **true**. |

## <a name="response-body"></a>Corpo da resposta

Se tiver êxito, este método retornará `HTTP/1.1 204 OK` o código de status.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/v1.0/domains/{id}/forceDelete
Content-type: application/json

{
  "disableUserAccounts": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-forcedelete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-forcedelete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-forcedelete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-forcedelete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/domain-forcedelete-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

