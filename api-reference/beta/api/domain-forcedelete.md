---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99ea7666050ba167503fe330bd1c4b9b48aff64b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655765"
---
# <a name="domain-forcedelete"></a>domínio: forceDelete

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclui um domínio usando uma operação assíncrona.

As ações a seguir são executadas como parte desta operação:

* Renomeia o UPN, o EmailAddress e o ProxyAddress de usuários com referências para o domínio excluído.

* Renomeia o EmailAddress de grupos com referências para o domínio excluído.

* Renomeia a Identifieruris agora de aplicativos com referências para o domínio excluído.

* Se o número de objetos a serem renomeados for maior que 1000, um erro será retornado.

* Se um dos aplicativos a ser renomeado for um aplicativo de vários locatários, um erro será retornado.

Após a conclusão da exclusão do domínio, as operações de API para o domínio excluído retornarão um código de resposta HTTP 404. Para verificar a exclusão de um domínio, você pode executar um [domínio Get](domain-get.md). Se o domínio tiver sido excluído com êxito, um código de resposta HTTP 404 será retornado na resposta.

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

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|disableUserAccounts|Booliano| Opção para desabilitar contas de usuário renomeadas. Se uma conta de usuário estiver desabilitada, o usuário não terá permissão para entrar.<br>*True* (padrão)-as contas de usuário renomeadas como parte dessa operação estão desabilitadas.<br>*False* -as contas de usuário renomeadas como parte dessa operação não estão desabilitadas. |

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK`. 

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
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

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_forcedelete-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
