---
title: Criar política
description: Crie um novo objeto de diretiva especificando o nome para exibição, tipo de política e descrição da política.
ms.openlocfilehash: fca6201d7afa6a78f15da0d37fb611e4114783e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040277"
---
# <a name="create-policy"></a>Criar política

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie um novo objeto de [diretiva](../resources/policy.md) especificando o nome para exibição, tipo de política e descrição da política.

>Observação: Os detalhes da diretiva serão validados antes de serem armazenados. Se ele não passar na validação, um 400 Solicitação incorreta será retornado.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

```http
POST /policies
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type | application/json  | Natureza dos dados no corpo de uma entidade. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornecem uma representação de JSON do objeto de [diretiva](../resources/policy.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você criar uma diretiva.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definição|String|A versão de cadeia de caracteres do objeto de [diretiva](../resources/policy.md) .|
|displayName|String|Um nome personalizado para a política.|
|type|String|Especifica o tipo de política. No momento deve ser "TokenLifetimePolicy"|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` objeto de código e a [diretiva](../resources/policy.md) de resposta no corpo da resposta. Se não obtiver êxito, uma `4xx` será retornado o erro com detalhes específicos.  

## <a name="example"></a>Exemplo
O exemplo a seguir cria uma nova vida útil do token política. Observe que o parâmetro de definição de cadeia de caracteres tem escape aspas duplas.

##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
