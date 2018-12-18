---
title: Força a exclusão de domínio
description: Exclui um domínio usando uma operação de longa execução assíncrona.
author: lleonard-msft
ms.openlocfilehash: 85839d8bf7d36925661d0202c053574288763dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309111"
---
# <a name="force-domain-deletion"></a>Força a exclusão de domínio

Exclui um domínio usando uma operação de longa execução assíncrona.

As seguintes ações são executadas como parte dessa operação:

* Atualizações de `userPrincipalName`, `mail`, e `proxyAddresses` propriedades de `users` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.

* Atualizações de `mail` propriedade do `groups` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.

* Atualizações de `identifierUris` propriedade do `applications` com referências ao domínio excluído para usar o domínio onmicrosoft.com inicial.

* Se o número de objetos a ser renomeado for maior que 1000, um erro será retornado.

* Se um do `applications` a ser renomeado é um aplicativo de multilocatário, será retornado um erro.

Após a exclusão de domínio for concluído, as operações de API para o domínio excluído retornará um código de status HTTP 404. Para verificar a exclusão de um domínio, você pode executar uma operação [obter o domínio](domain-get.md) .

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

| Parâmetro | Type | Descrição |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| Opção para desabilitar contas de usuário que são renomeadas. Se uma conta de usuário estiver desabilitada, o usuário não poderão entrar. Se definida como **true** o `users` atualizados como parte dessa operação será desabilitado.  Valor padrão é **true**. |

## <a name="response-body"></a>Corpo da resposta

Se tiver êxito, este método retornará `HTTP/1.1 204 OK` código de status.

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->