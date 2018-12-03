---
title: 'domínio: forceDelete'
description: Exclui um domínio usando uma operação assíncrona.
ms.openlocfilehash: 590ba49a4aff99385a2584b3d544d7682a030eb6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034569"
---
# <a name="domain-forcedelete"></a>domínio: forceDelete

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Exclui um domínio usando uma operação assíncrona.

As seguintes ações são executadas como parte dessa operação:

* Renomeia o UPN, EmailAddress e ProxyAddress de usuários com referências ao domínio excluído.

* Renomeia os EmailAddress dos grupos com referências ao domínio excluído.

* Renomeia o identifierUris de aplicativos com referências ao domínio excluído.

* Se o número de objetos a ser renomeado for maior que 1000, um erro será retornado.

* Se nenhum dos aplicativos a ser renomeado é um aplicativo de multilocatário, um erro será retornado.

Após a exclusão de domínio for concluído, as operações de API para o domínio excluído retornará um código de resposta HTTP 404. Para verificar a exclusão de um domínio, você pode executar um [domínio de obter](domain-get.md). Se o domínio foi excluído com êxito, será retornado um código de resposta HTTP 404 na resposta.

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
|disableUserAccounts|Booliano| Opção para desabilitar contas de usuário renomeado. Se uma conta de usuário estiver desabilitada, o usuário não poderão entrar.<br>*True* (padrão) - usuário renomeadas como parte desta operação de contas estão desabilitadas.<br>*False* - contas de usuário renomeadas como parte desta operação não estejam desabilitados. |

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->