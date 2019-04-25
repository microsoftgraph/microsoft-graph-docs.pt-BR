---
title: 'group: delta'
description: Obter grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação de grupo, sem ter que executar uma leitura completa de toda a coleção de grupos. Consulte usando a consulta Delta para obter detalhes.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 344b9745a998dcfb1107a1af72691184732718b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522598"
---
# <a name="group-delta"></a>group: delta
Obter grupos recém-criados, atualizados ou excluídos, incluindo alterações de associação de grupo, sem ter que executar uma leitura completa de toda a coleção de grupos. Consulte [usando a consulta Delta](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para iniciar o rastreamento de alterações, faça uma solicitação incluindo a função delta no recurso de grupos.

<!-- { "blockType": "ignored" } -->

```http
GET /groups/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações em grupos resulta em uma rodada de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e de `$skiptoken`), especifique na solicitação inicial **delta**. O Microsoft Graph codifica automaticamente os parâmetros especificados para a parte de token da URL `nextLink` ou `deltaLink` fornecida na resposta.

Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.

Em solicitações subsequentes, copie e aplique a URL `nextLink` ou `deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta | Tipo  |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de grupos indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de grupos. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Este método oferece suporte a parâmetros de consulta OData opcionais para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade *id* sempre será retornada.
- Você pode usar `$expand=members` o para obter alterações de associação.
- Há suporte limitado para `$filter`:
  - A única expressão `$filter` suportada é para controlar alterações em um objeto específico: `$filter=id+eq+{value}`. É possível filtrar vários objetos. Por exemplo, `https://graph.microsoft.com/v1.0/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ffff' or id eq '004d6a07-fe70-4b92-add5-e6e37b8affff'`. Há um limite de 50 objetos filtrados.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |
| Preferir | retorno = mínimo <br><br>A especificação desse cabeçalho com uma solicitação que usa `deltaLink` um retornava apenas as propriedades do objeto que foram alteradas desde a última rodada. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta. A resposta também inclui um token de estado que é uma `nextLink` URL ou uma `deltaLink` URL.

- Se uma `nextLink` URL for retornada:
  - Isso indica que há outras páginas de dados a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.
  - A resposta inclui o mesmo conjunto de propriedades que na solicitação de consulta Delta inicial. Isso permite que você capture o estado atual completo dos objetos ao iniciar o ciclo Delta.

- Se uma `deltaLink` URL for retornada:
  - Isso indica que não há mais dados sobre o estado existente do recurso a ser retornado. Salve e use a `deltaLink` URL para saber mais sobre as alterações no recurso na próxima rodada.
  - Você tem a opção de especificar o `Prefer:return=minimal` cabeçalho, para incluir os valores de resposta somente para as propriedades que foram alteradas desde o momento `deltaLink` em que foi emitido.

#### <a name="default-return-the-same-properties-as-initial-delta-request"></a>Padrão: retornar as mesmas propriedades que a solicitação Delta inicial

Por padrão, as solicitações usando `deltaLink` uma `nextLink` ou retornam as mesmas propriedades selecionadas na consulta Delta inicial das seguintes maneiras:

- Se a propriedade tiver sido alterada, o novo valor será incluído na resposta. Isso inclui propriedades que estão sendo definidas como valor nulo.
- Se a propriedade não tiver sido alterada, o valor antigo será incluído na resposta.
- Se a propriedade nunca tiver sido definida antes de não ser incluída na resposta.


> **Observação:** Com esse comportamento, observando a resposta, não é possível dizer se uma propriedade está sendo alterada ou não. Além disso, as respostas Delta tendem a ser grandes porque elas contêm todos os valores de propriedade, conforme mostrado no [segundo exemplo](#request-2) abaixo.

#### <a name="alternative-return-only-the-changed-properties"></a>Alternativa: retornar somente as propriedades alteradas

Adicionar um cabeçalho de solicitação opcional `prefer:return=minimal` --resulta no seguinte comportamento:

- Se a propriedade tiver sido alterada, o novo valor será incluído na resposta. Isso inclui propriedades que estão sendo definidas como valor nulo.
- Se a propriedade não tiver sido alterada, a propriedade não será incluída na resposta. (Diferente do comportamento padrão.)

> **Observação:** O cabeçalho pode ser adicionado a uma `deltaLink` solicitação em um determinado momento no ciclo Delta. O cabeçalho afeta apenas o conjunto de propriedades incluído na resposta e não afeta como a consulta Delta é executada. ConFira o [terceiro exemplo](#request-3) abaixo.

### <a name="example"></a>Exemplo

#### <a name="request-1"></a>Solicitação 1

Este é um exemplo de solicitação. Não há nenhum `$select` parâmetro, portanto, um conjunto padrão de propriedades é rastreado e retornado.
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta
```

#### <a name="response-1"></a>Resposta 1

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta.

>**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade. Todas as propriedades serão retornadas de uma chamada real.
>
> Observe a presença da propriedade *Members @ Delta* que inclui as IDs dos objetos member no grupo.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups","@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjvY1FSSc_",
  "value":[
    {
      "classification": "classification-value",
      "createdDateTime":"datetime-value",
      "description":"Test group 1",
      "displayName":"TestGroup1",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "members@delta": [
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "693acd06-2877-4339-8ade-b704261fe7a0"
               },
               {
                   "@odata.type": "#microsoft.graph.user",
                   "id": "49320844-be99-4164-8167-87ff5d047ace"
               }
      ]
    }
  ]
}
```

#### <a name="request-2"></a>Solicitação 2

O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para o controle de alterações, com comportamento de resposta padrão:
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
```

#### <a name="response-2"></a>Resposta 2

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta. Observe que todas as 3 propriedades estão incluídas na resposta e não são conhecidas quais foram alteradas desde que `deltaLink` foram obtidas.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null,
      "mailNickname": "mailNickname-value"
    }
  ]
}
```

#### <a name="request-3"></a>Solicitação 3

O exemplo a seguir mostra a solicitação inicial selecionando 3 Propriedades para controle de alterações, com comportamento de resposta mínimo alternativo:
<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/delta?$select=displayName,description,mailNickname
Prefer: return=minimal
```

#### <a name="response-3"></a>Resposta 3

Veja a seguir um exemplo da resposta ao usar `deltaLink` obtido da inicialização da consulta. Observe que a `mailNickname` propriedade não é incluída, o que significa que ela não foi alterada desde a última consulta Delta; `displayName` e `description` são incluídos, o que significa que seus valores foram alterados.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "displayName": "displayName-value",
      "description": null
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Usar a consulta Delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).
- [Obter alterações incrementais para grupos](/graph/delta-query-groups).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
