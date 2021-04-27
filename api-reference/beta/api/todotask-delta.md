---
title: 'todoTask: delta'
description: Obter um conjunto de recursos todoTask que foram adicionados, excluídos ou atualizados em um todoTaskList especificado.
localization_priority: Normal
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3c0d1759d1994c1fa9ae405d2a1895982e3ac99a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048915"
---
# <a name="todotask-delta"></a>todoTask: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um conjunto de [recursos todoTask](../resources/todotask.md) que foram adicionados, excluídos ou atualizados em [um todoTaskList especificado.](../resources/todotasklist.md)

Uma **chamada** de função delta para recursos **todoTask** em **um todoTaskList** é semelhante a uma solicitação GET, exceto que, aplicando [adequadamente tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTask** em **todoTaskList**. Isso permite manter e sincronizar um armazenamento local dos recursos **todoTask** de um usuário sem precisar buscar todo o conjunto do servidor sempre.  

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Tasks.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Tasks.ReadWrite    |
|Aplicativo | Sem suporte |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/todo/lists/{id}/tasks/delta
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações em uma **coleção todoTask** incorre em uma rodada de uma ou mais chamadas de **função delta.** Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção `deltaLink` todoTask, indicando a conclusão dessa rodada de controle de alterações.  Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção `nextLink` todoTask.  |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 
- Suporte à consulta `$select` delta , e para `$top` `$expand` todoTask. 
- Há suporte limitado para `$filter` e `$orderby`:
  * As únicas expressões `$filter` com suporte são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.
  * A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida. 
- Não há suporte para `$search`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [todoTask](../resources/todotask.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Para controlar as alterações nos recursos **todoTask** em um **todoTaskList** desde a última rodada de controle de alterações, você faria uma ou mais chamadas de função **delta** para obter o conjunto de alterações incrementais. O exemplo a seguir mostra como iniciar uma próxima rodada de controle de alterações, usando a URL na chamada de última função delta da última rodada, que contém `deltaLink` um  `deltaToken` . Essa **chamada** de função delta limita o número máximo de **todoTask** no corpo da resposta como 2.
 

### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
Prefer: odata.maxpagesize=2
```


### <a name="response"></a>Resposta
Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_  
(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.

A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.

Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 337

{
   "@odata.deltaLink":"https://graph.microsoft.com/beta/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
   "value":[
      {
         "@odata.etag":"W/\"4rfRVIPi9EqXgDbc8U7HGwADLLQ9xQ==\"",
         "importance":"normal",
         "isReminderOn":false,
         "status":"notStarted",
         "title":"empty task3",
         "createdDateTime":"2020-08-12T04:54:29.1925206Z",
         "lastModifiedDateTime":"2020-08-12T04:54:29.4903939Z",
         "id":"AAMkADMwNTcyZjQzLTdkMGItNDdjMy04ZTYwLTJhYmUzNGI5ZDEwMwBGAAAAAAB5M0K0qlJySLOAgV22zPnuBwDit9FUg_L0SpeANtzxTscbAAMNmhwmAADit9FUg_L0SpeANtzxTscbAAMxlnrYAAA=",
         "body":{
            "content":"",
            "contentType":"text"
         }
      }
   ]
}
```

## <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](/graph/delta-query-overview)

