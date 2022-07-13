---
title: 'todoTaskList: delta'
description: Obtenha um conjunto de recursos todoTaskList que foram adicionados, excluídos ou removidos no Microsoft To Do.
ms.localizationpriority: medium
author: avijityadav
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ff97063f53297ca2457252aae5dec3b1dfd42c18
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66767943"
---
# <a name="todotasklist-delta"></a>todoTaskList: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha um conjunto de [recursos todoTaskList](../resources/todotasklist.md) que foram adicionados, excluídos ou removidos no Microsoft To Do.

Uma **chamada** de função delta para **todoTaskList** é semelhante a uma solicitação GET, exceto que, aplicando adequadamente [tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais no **todoTaskList**. Isso permite que você mantenha e sincronize um repositório local de **todoTaskList** de um usuário sem precisar buscar todas as **tarefas do todoTaskList** do servidor todas as vezes.

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
GET /me/todo/lists/delta
GET /users/{id|userPrincipalName}/todo/lists/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O acompanhamento de alterações **nos recursos todoTaskList** incorre em uma rodada de uma ou mais **chamadas de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Nas solicitações subsequentes, `@odata.nextLink` `@odata.deltaLink` basta copiar e aplicar a URL da resposta anterior, pois essa URL já inclui os parâmetros codificados e desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado `@odata.deltaLink` na URL da chamada de função **delta anterior** para a mesma coleção **todoTaskList** , indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `@odata.deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado `@odata.nextLink` na URL da chamada de função **delta** anterior, indicando que há mais alterações a serem controladas na mesma **coleção todoTaskList** . |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

> **Nota:** No cabeçalho da solicitação, o valor deve `odata.maxpagesize` ser maior ou igual a 10 para obter o valor `nextLink` correto.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e [um objeto de coleção todoTaskList](../resources/todotasklist.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir mostra como fazer uma chamada de função **delta inicial** e limitar o número máximo de **todoTaskList** no corpo da resposta a 2.

Para controlar as alterações no **todoTaskList**, você faria uma ou mais chamadas de função **delta** , com tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta. 

As principais diferenças entre acompanhar **todoTaskList** e acompanhar recursos **de todoTask** em uma lista estão nas URLs de solicitação de consulta delta e as respostas de consulta retornando **todoTaskList** em vez de coleções **todoTask** .

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/delta
Prefer: odata.maxpagesize=12
```
### <a name="response"></a>Resposta

Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_  
(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.

A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

```http
HTTP/1.1 200 OK
Content-type: application/json

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

