---
title: 'todoTask: delta'
description: Obtenha um conjunto de recursos todoTask que foram adicionados, excluídos ou atualizados em um todoTaskList especificado.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f7e789de85a19fbbb41308e68f7a4d71a03f6919
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246934"
---
# <a name="todotask-delta"></a>todoTask: delta

Namespace: microsoft.graph

Obtenha um conjunto de [recursos todoTask](../resources/todotask.md) que foram adicionados, excluídos ou atualizados em um [todoTaskList especificado](../resources/todotasklist.md).

Uma **chamada** de função delta para recursos **todoTask** em um **todoTaskList** é semelhante a uma solicitação GET, exceto que, aplicando [adequadamente tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTask** nesse **todoTaskList**. Isso permite que você mantenha e sincronize um repositório local dos recursos **todoTask** de um usuário sem precisar buscar todo o conjunto do servidor toda vez.  

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

O controle de alterações em **uma coleção todoTask** incorre em uma rodada de uma ou mais **chamadas de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Nas solicitações subsequentes, `@odata.nextLink` `@odata.deltaLink` basta copiar e aplicar a URL da resposta anterior, pois essa URL já inclui os parâmetros codificados e desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `@odata.deltaLink` URL da chamada de função **delta anterior** para a mesma coleção todoTask, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `@odata.deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.nextLink` URL da chamada de função **delta anterior** , indicando que há mais alterações a serem controladas na mesma coleção todoTask. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 
- Suporte a consultas delta `$select`e `$top`todoTask `$expand` . 
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

Se bem-sucedido, este método retorna um código `200 OK` de resposta e [um objeto de coleção todoTask](../resources/todotask.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Para controlar as alterações nos recursos **todoTask** em um **todoTaskList** desde a última rodada de controle de alterações, você faria uma ou mais chamadas de função **delta** para obter o conjunto de alterações incrementais. O exemplo a seguir mostra como iniciar uma próxima rodada de controle de alterações, usando a URL `@odata.deltaLink` retornada da última chamada de função **delta** da última rodada, que contém um `deltaToken`. Essa **chamada** de função delta limita o número máximo de **todoTask** no corpo da resposta a 2.
 

### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=w0vf2jHg2mBXU-I2AK0FSWl0dopNtG8u5YoM
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

{
   "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/todo/lists/gDbc8U7HGwADDZocJgAAAA==/tasks/delta?$deltatoken=MoVMZ_DzHG4AhT3WE8VioVS1IXZJ-ArqK5fknOjnKFY",
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

