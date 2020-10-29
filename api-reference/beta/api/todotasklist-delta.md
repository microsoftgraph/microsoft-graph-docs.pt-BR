---
title: 'todoTaskList: Delta'
description: Obtenha um conjunto de recursos do todoTaskList que foram adicionados, excluídos ou removidos no Microsoft para o.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9719b4c9379a79172cc4052439dc4e8abb72b716
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796581"
---
# <a name="todotasklist-delta"></a>todoTaskList: Delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha um conjunto de recursos do [todoTaskList](../resources/todotasklist.md) que foram adicionados, excluídos ou removidos no Microsoft para o.

Uma chamada de função **Delta** para **todoTaskList** é semelhante a uma solicitação GET, exceto pelo fato de que, por meio da aplicação adequada de [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTaskList** . Isso permite que você mantenha e sincronize um repositório local do **todoTaskList** de um usuário sem ter que buscar todo o **todoTaskList** do servidor a cada vez.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Tasks.ReadWrite    |
|Delegada (conta pessoal da Microsoft) | Tasks.ReadWrite    |
|Aplicativo | Sem suporte |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações nos recursos do **todoTaskList** provoca uma rodada de uma ou mais chamadas de função **Delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta** . O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, basta copiar e aplicar `nextLink` a `deltaLink` URL ou da resposta anterior, pois essa URL já inclui os parâmetros codificados e desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção **todoTaskList** , indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção **todoTaskList** . |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto da coleção [todoTaskList](../resources/todotasklist.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir mostra como fazer uma chamada de função **Delta** inicial e limitar o número máximo de **todoTaskList** no corpo da resposta a 2.

Para controlar as alterações no **todoTaskList** , faça uma ou mais chamadas de função **Delta** , com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta Delta. 

As principais diferenças entre o acompanhamento de **todoTaskList** e o acompanhamento de recursos do **todoTask** em uma lista estão nas URLs de solicitação de consulta Delta e as respostas de consulta retornando **TodoTaskList** em vez de conjuntos **todoTask** .

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=2
```
### <a name="response"></a>Resposta

Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_  
(em um cabeçalho de resposta _@odata.nextLink_ ) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_ ). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.

A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_ .

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/delta?$skiptoken=ldfdgdgfoT5csv4k99nvQqyku0jaGqMhc6XyFff5qQTQ7RJOr",
  "value": [
    {
      "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ93w==\"",
         "displayName":"List1",
         "isOwner":true,
         "isShared":false,
         "wellknownListName":"none",
         "id":"AQMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZD"
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](/graph/delta-query-overview)

