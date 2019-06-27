---
title: Forçar exclusão de domínio
description: Exclui um domínio usando uma operação assíncrona de execução longa.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 249f58a9728b349c5b00000e18d2491158e95936
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272181"
---
# <a name="force-domain-deletion"></a>Forçar exclusão de domínio

Exclui um domínio usando uma operação assíncrona de execução longa.

As ações a seguir são executadas como parte desta operação:

* Atualiza as `userPrincipalName`propriedades `mail`, e `proxyAddresses` de `users` com referências para o domínio excluído para usar o domínio onmicrosoft.com inicial.

* Atualiza a `mail` propriedade de `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.

* Atualiza a `identifierUris` propriedade de `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.

* Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.

* Se um dos `applications` a ser renomeado for um aplicativo de vários locatários, um erro será retornado.

Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de status HTTP 404. Para verificar a exclusão de um domínio, você pode executar uma operação [Get Domain](domain-get.md) .

## <a name="permissions"></a>Permissões

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

| Nome | Descrição |
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro | Tipo | Descrição |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Opção para desabilitar as contas de usuário que são renomeadas. Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar. Se definido como **true** , `users` a parte atualizada como parte dessa operação será desabilitada.  O valor padrão é **true**. |

## <a name="response-body"></a>Corpo da resposta

Se bem-sucedido, este método retorna `HTTP/1.1 204 OK` o código de status.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
