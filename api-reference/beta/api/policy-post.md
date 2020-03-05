---
title: Criar política
description: Criar um novo objeto de política especificando o nome de exibição, o tipo de política e a descrição da política.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2e13ef2bdcf424d68d94d97412487708022386cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455498"
---
# <a name="create-policy"></a>Criar política

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto de [política](../resources/policy.md) especificando o nome de exibição, o tipo de política e a descrição da política.

>Observação: os detalhes da política serão validados antes de serem armazenados. Se ele não passar na validação, uma solicitação inválida 400 será retornada.

## <a name="permissions"></a>Permissões
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
No corpo da solicitação, forneça uma representação JSON do objeto [Policy](../resources/policy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar uma política.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definir|String|A versão de cadeia de caracteres do objeto [Policy](../resources/policy.md) .|
|displayName|Cadeia de caracteres|Um nome personalizado para a política.|
|type|String|Especifica o tipo de política. No momento, deve ser "TokenLifetimePolicy"|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Policy](../resources/policy.md) no corpo da resposta. Caso não consiga, um `4xx` erro será retornado com detalhes específicos.  

## <a name="example"></a>Exemplo
O exemplo a seguir cria uma nova política de tempo de vida do token. Observe que o parâmetro de definição de cadeia de caracteres tem aspas duplas de escape.

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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
