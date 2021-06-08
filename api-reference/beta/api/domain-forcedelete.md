---
title: 'domain: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47f81a25fc29f6a7eb0bb79c0f4d84e37825183a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786822"
---
# <a name="domain-forcedelete"></a>domain: forceDelete

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclui um domínio usando uma operação assíncrona.

Antes de chamar [forceDelete](domain-forcedelete.md), você deve atualizar ou remover quaisquer referências **Exchange** como o serviço de provisionamento.

As seguintes ações são executadas como parte desta operação:

* Renomeia o UPN, EmailAddress e ProxyAddress de usuários com referências ao domínio excluído.

* Renomeia o EmailAddress de grupos com referências ao domínio excluído.

* Renomeia os identificadores de aplicativos com referências ao domínio excluído.

* Se o número de objetos a serem renomeados for maior que 1.000, um erro será retornado.

* Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.

Depois que a exclusão de domínio for concluída, as operações de API do domínio excluído retornarão um código de resposta HTTP 404. Para verificar a exclusão de um domínio, você pode executar um [domínio get](domain-get.md). Se o domínio foi excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Domain.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|disableUserAccounts|Booliano| Opção para desabilitar contas de usuário renomeadas. Se uma conta de usuário estiver desabilitada, o usuário não poderá entrar.<br>*True* (padrão) - As contas de usuário renomeadas como parte dessa operação estão desabilitadas.<br>*False* - As contas de usuário renomeadas como parte dessa operação não estão desabilitadas. |

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK`. 

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

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

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


