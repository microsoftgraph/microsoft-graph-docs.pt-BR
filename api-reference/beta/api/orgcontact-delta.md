---
title: 'orgContact: Delta'
description: Obter contatos organizacionais recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b30df74f4b479fac08d36a3983939d51d9c52bd
ms.sourcegitcommit: 2ac179fb774a15c9e9c01502e59c76efb57803a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2020
ms.locfileid: "42986300"
---
# <a name="orgcontact-delta"></a>orgContact: Delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter contatos organizacionais recém-criados, atualizados ou excluídos sem ter que realizar uma leitura completa de toda a coleção. Confira [Controlar alterações](/graph/delta-query-overview) para saber mais.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.  |
|Application | OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar as alterações, faça uma solicitação incluindo a função Delta no recurso contatos.

<!-- { "blockType": "ignored" } -->
```http
GET /contacts/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em contatos organizacionais provoca uma rodada de uma ou mais chamadas de função **Delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.

Você só precisa especificar qualquer parâmetro de consulta uma vez na frente.

Em solicitações subsequentes, copie e aplique `nextLink` a `deltaLink` URL ou à resposta anterior. Essa URL já inclui os parâmetros codificados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para o mesmo conjunto de contatos da organização, indicando a conclusão da rodada de controle de alterações. Salve e aplique a URL `deltaLink` inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle de alterações para essa coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de contatos da organização. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Este método oferece suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.

- Você pode usar um `$select` parâmetro de consulta como em qualquer solicitação get para especificar apenas as propriedades que você precisa para o melhor desempenho. A propriedade **id** sempre será retornada.
- Há suporte limitado para `$filter`:
  - A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`. É possível filtrar vários objetos. Por exemplo, `https://graph.microsoft.com/beta/contacts/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Há um limite de 50 objetos filtrados.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;token&gt; de portador. Obrigatório.|
| Preferir | return=minimal <br><br>Especificar esse cabeçalho com uma solicitação que usa `deltaLink` retorna somente as propriedades do objeto que foram alteradas desde a última vez. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [orgContact](../resources/orgcontact.md) no corpo da resposta. A resposta também inclui uma URL `nextLink` ou `deltaLink`.

- Se uma URL `nextLink` for retornada:
  - Existem páginas de dados adicionais a recuperar na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.
  - A resposta inclui o mesmo conjunto de propriedades como na solicitação de consulta delta inicial. Assim você pode capturar o estado atual de todos os objetos ao iniciar o ciclo de delta.

- Se uma URL `deltaLink` for retornada:
  - Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado. Salve e use a URL `deltaLink` para saber mais sobre alterações ao recurso na próxima fase.
  - Você pode especificar o cabeçalho `Prefer:return=minimal` para incluir somente os valores de resposta das propriedades que foram alteradas desde a hora em que o `deltaLink` foi emitido.

### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Padrão: retornar as mesmas propriedades de uma solicitação delta inicial

Por padrão, as solicitações usando `deltaLink` ou `nextLink` retornam as mesmas propriedades selecionadas na consulta delta inicial das seguintes maneiras:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, o valor antigo será incluído na resposta.
- Se a propriedade nunca tiver sido definida antes, ela não será incluída na resposta.


> **Observação:** Com esse comportamento, não é possível dizer se uma propriedade está mudando observando a resposta. Além disso, as respostas Delta tendem a ser grandes porque elas contêm todos os valores de propriedade, conforme mostrado no [exemplo 2](#example-2-selecting-three-properties).

### <a name="alternative-return-only-the-changed-properties"></a>Alternativa: retornar somente as propriedades alteradas

Adicionar o cabeçalho `prefer:return=minimal` opcional na solicitação resulta no comportamento a seguir:

- Se a propriedade foi alterada, o novo valor será incluído na resposta. Isso inclui propriedades definidas com valor nulo.
- Se a propriedade não foi alterada, a propriedade não será incluído na resposta de forma alguma. (Diferente do comportamento padrão.)

> **Observação:** é possível adicionar o cabeçalho a uma solicitação `deltaLink` a qualquer momento no ciclo de delta. O cabeçalho afeta apenas o conjunto de propriedades incluído na resposta e não afeta como a consulta Delta é executada. Veja o [Exemplo 3](#example-3-alternative-minimal-response-behavior).

## <a name="examples"></a>Exemplos

### <a name="example-1-default-properties"></a>Exemplo 1: Propriedades padrão

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Como não há nenhum `$select` parâmetro, um conjunto padrão de propriedades é rastreado e retornado.

<!-- {
  "blockType": "request",
  "name": "orgContact_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta
```


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "id": "string (identifier)",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mailNickname": "mailNickname-value",
      "surname": "surname-value"
    }
  ]
}
```

### <a name="example-2-selecting-three-properties"></a>Exemplo 2: Escolher três propriedades

#### <a name="request"></a>Solicitação

O próximo exemplo mostra uma solicitação inicial selecionando três propriedades para controle de alterações com comportamento de resposta padrão.

<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_select"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
```

#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que todas as três propriedades foram incluídas na resposta e não se sabe quais foram alteradas desde que o `deltaLink` foi obtido.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": "jobTitle-value",
      "mail": null
    }
  ]
}
```

### <a name="example-3-alternative-minimal-response-behavior"></a>Exemplo 3: Comportamento de resposta mínimo alternativo

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação inicial selecionando três propriedades para controle de alterações com o comportamento de resposta mínima alternativa.

<!-- {
  "blockType": "request",
  "name": "orgcontact_delta_minimal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/delta?$select=displayName,jobTitle,mail
Prefer: return=minimal
```

#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta ao usar `deltaLink` obtido da inicialização de consulta. Observe que a `mail` propriedade não é incluída, o que significa que ela não foi alterada desde a última consulta Delta; `displayName` e `jobTitle` são incluídos, o que significa que seus valores foram alterados.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#contacts",
  "@odata.nextLink":"https://graph.microsoft.com/beta/contacts/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "jobTitle": null
    }
  ]
}
```
## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).

<!-- uuid: 3B5A9A7C-6324-432F-8C66-AC4883DD71EF
2020-03-20 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
