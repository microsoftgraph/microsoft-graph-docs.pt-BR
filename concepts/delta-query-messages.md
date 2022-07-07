---
title: Obter as alterações incrementais para as mensagens em uma pasta
description: Use a consulta delta para controlar as alterações de mensagens em uma hierarquia de pastas acompanhando cada pasta individualmente. O exemplo mostra como sincronizar mensagens em uma pasta.
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 06e4b6787a298ef245323b84671c0716768751fb
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671392"
---
# <a name="get-incremental-changes-to-messages-in-a-folder"></a>Obter as alterações incrementais para as mensagens em uma pasta

A consulta delta permite consultar adições, exclusões ou atualizações de mensagens em uma pasta, por meio de uma série de chamadas de função [delta](/graph/api/message-delta). Os dados delta permitem manter e sincronizar um armazenamento local de mensagens do usuário, sem ter de buscar todo o conjunto de mensagens do usuário no servidor a cada vez que precise deles.

A consulta delta oferece suporte à sincronização completa, que recupera todas as mensagens em uma pasta (por exemplo, a Caixa de Entrada do usuário), e à sincronização incremental, que recupera todas as mensagens que foram alteradas nessa pasta desde a última sincronização. Normalmente, você faria uma sincronização completa inicial de todas as mensagens em uma pasta e, logo após, obteria alterações incrementais para essa pasta periodicamente.

## <a name="track-message-changes-in-a-folder"></a>Controlar mensagens de alterações em uma pasta

A consulta delta é uma operação por pasta. Para controlar as alterações das mensagens em uma hierarquia de pastas, você precisa controlar cada pasta individualmente.

O rastreamento de alterações de mensagem em uma paste de email corresponde a uma série de solicitações GET com a função **delta**. A solicitação GET inicial é muito semelhante à maneira como você [obtém mensagens](/graph/api/user-list-messages), exceto se você incluir a função **delta**:

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages/delta
```

Uma solicitação GET com a função **delta** retorna:

- Uma `@odata.nextLink` (que contém uma URL com chamada de função **delta** e um _skipToken_) ou
- Uma `@odata.deltaLink` (que contém uma URL com chamada de função **delta** e _deltaToken_).

Esses tokens são [tokens de estado](delta-query-overview.md#state-tokens) que são completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL retornada da última solicitação GET para a próxima chamada de função **delta** da mesma pasta. Um `@odata.deltaLink` retornado em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `@odata.deltaLink` quando começar a próxima fase.

Verifique o `@odata.nextLink`exemplo`@odata.deltaLink` para aprender a usar as URLs [ e ](#example-synchronize-messages-in-a-folder).

### <a name="use-query-parameters-in-a-delta-query-for-messages"></a>Use os parâmetros de consulta em uma consulta delta para mensagens

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade `id` sempre será retornada.
- Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens.
- Há suporte limitado para `$filter` e `$orderby`:
  - As únicas expressões `$filter` com suporte são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.
  - A aplicação de `$filter` em uma consulta Delta retorna apenas até 5.000 mensagens.
  - A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida.
- Não há suporte para `$search`.

### <a name="optional-request-header"></a>Cabeçalhos de solicitação opcionais

Cada solicitação GET de consulta delta retorna um conjunto de um ou mais mensagens na resposta. Como alternativa, você pode especificar o cabeçalho de solicitação, `Prefer: odata.maxpagesize={x}`, para configurar o máximo de mensagens em uma resposta.

<!--
### Iterative process

A typical round to track message changes goes like this:

1. Make the initial GET request with the mandatory _Prefer: odata.track-changes_ header. If this is your very first delta query
for messages in that folder, don't provide any state token. If the messages support tracking changes, following the iterative
process (steps 2-6) described below will return the entire set of messages in that folder.

2. Check if the first response returns the _Preference-Applied: odata.track-changes_ header,
which confirms your resource supports tracking changes. Stop if you don't receive the response header.

3. If you receive a _skipToken_ (in an _@odata.nextLink_ response header) in the response, you should continue to track the
   additional messages that have changed (added, deleted, or updated). Make a second GET request, using the URL returned
   in _@odata.nextLink_, which includes a _skipToken_.

4. The second request will return additional messages that have changed, and either a _skipToken_ if there are more changed messages,
  or a _deltaToken_ if all the changed messages have been returned.

5. If you receive a _skipToken_ from the last GET request, continue getting the changes by sending a next GET call, similar to step 3.

6. When you eventually receive a _deltaToken (in an _@odata.deltaLink_ response header) in the response from a GET, stop. This
round of change tracking is complete.

7. Save the _deltaToken_. The next time you track changes for the same folder, make a GET request
similar to step 1, except that now you can use this _deltaToken_ to get just the delta data (messages that have been added, deleted or updated)
since the completion of the very first round.

-->

## <a name="example-synchronize-messages-in-a-folder"></a>Exemplo: sincronizar mensagens em uma pasta

O exemplo a seguir mostra 2 sessões de sincronização de uma pasta específica que, inicialmente, contém 5 mensagens.

A primeira sessão envolve uma série de 3 solicitações para sincronizar todas as 5 mensagens na pasta:

- [Solicitação inicial de exemplo](#sample-initial-request) e [resposta](#sample-initial-response)
- [Solicitação de segundo exemplo](#sample-second-request) e [resposta](#sample-second-response)
- [Terceiro exemplo de solicitação](#sample-third-request) e [resposta final](#sample-third-and-final-response)

Após a primeira sessão, uma das mensagens é excluída e outra é marcada como lida. A [segunda sessão](#synchronize-messages-in-the-same-folder-in-the-next-round) da sincronização retorna apenas o intervalo (a exclusão e atualização) sem retornar as demais mensagens que permaneceram as mesmas.

### <a name="sample-initial-request"></a>Solicitação inicial de exemplo

Neste exemplo,a pasta especificada está sendo sincronizada pela primeira vez, para que a solicitação de sincronização inicial não inclua nenhum token de estado. Esta fase retornará todas as mensagens nessa pasta.

A primeira solicitação especifica o seguinte:

- Um parâmetro `$select` para retornar as propriedades `subject`, `sender` e `isRead` de cada mensagem na resposta.
- O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 mensagens de cada vez.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_1"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$select=subject,sender,isRead HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-initial-response"></a>Resposta inicial de exemplo

A resposta inclui duas mensagens e um cabeçalho de resposta `@odata.nextLink`. A URL `@odata.nextLink` indica que há mais mensagens na pasta para obter.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": false,
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB/\"",
      "subject": "Holiday promotion sale",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Samantha Booth",
          "address": "samanthab@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAVRMKAAAAA=="
    }
  ]
}
```

### <a name="sample-second-request"></a>Segundo exemplo de solicitação

A segunda solicitação especifica a URL `@odata.nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar o mesmo parâmetro `$select` como na solicitação inicial, pois o `skipToken` na URL `@odata.nextLink` os codifica e inclui.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_2"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPuoTQWfcsAbkYM HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-second-response"></a>Segunda resposta de exemplo

A segunda resposta retorna as 2 próximas mensagens na pasta e outro `@odata.nextLink`, indicando que há mais mensagens a ser lidas na pasta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlqfdAAAEfYB+\"",
      "subject": "Microsoft Virtual Academy at Contoso",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Elliot Hyde",
          "address": "elliot-hyde@tailspintoys.com"
        }
      },
      "id": "AQMkADNkNAAAgWkAAAA"
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "New or modified user account information",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Randi Welch",
          "address": "randiw@contoso.onmicrosoft.com"
        }
      },
      "id": "AQMkADNkNAAAgWJAAAA"
    }
  ]
}
```

### <a name="sample-third-request"></a>Terceira solicitação de exemplo

A terceira solicitação continua a usar a última URL do `@odata.nextLink` retornada da última solicitação de sincronização.

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_3"
}-->
```
GET https://graph.microsoft.com/v1.0/me/mailFolders/AQMkADNkNAAAgEMAAAA/messages/delta?$skiptoken=GwcBoTmPKILK4jLH7mAd1lLU HTTP/1.1
Prefer: odata.maxpagesize=2
```

### <a name="sample-third-and-final-response"></a>Terceira e última resposta de exemplo

A terceira resposta retorna a única mensagem restante em uma pasta, e uma URL `@odata.deltaLink` que indica que a sincronização está, por enquanto, concluída para esta pasta. Salvar e usar a URL `@odata.deltaLink` para [sincronizar a mesma pasta na próxima fase](#synchronize-messages-in-the-same-folder-in-the-next-round).

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzFPjSbaPPxzjlzOTAAAEfYB+\"",
      "subject": "Fabric CDN now available",
      "isRead": true,
      "sender": {
        "emailAddress": {
          "name": "Jodie Sharp",
          "address": "Jodie.Sharp@contoso.com"
        }
      },
      "id": "AAMkADk0MGFkODE3LWEAAA="
    }
  ]
}
```

### <a name="synchronize-messages-in-the-same-folder-in-the-next-round"></a>Sincronizar mensagens na mesma pasta na próxima sessão

Usando o `@odata.deltaLink` da [última solicitação](#sample-third-request) na última fase, você poderá obter somente as mensagens que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse nessa pasta desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AQMkADNkNAAAgEMAAAA"],
  "name": "get_messages_delta_next"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/mailfolders/AQMkADNkNAAAgEMAAAA/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY HTTP/1.1
Prefer: odata.maxpagesize=2
```

A resposta contém um `@odata.deltaLink`. Isso indica que todas as alterações na pasta de email remoto agora estão sincronizadas. Uma mensagem foi excluída e a mensagem foi alterada.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(message)",
  "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/mailfolders('AQMkADNkNAAAgEMAAAA')/messages/delta?$deltatoken=GwcBoTmPuoGNlgXgF1nyUNMXY",
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
      "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS0Dh_6qB-pB2Sa2pUum19a6YAAKnLuxoAAA=",
      "@removed": {
        "reason": "deleted"
      }
    },
    {
      "@odata.type": "#microsoft.graph.message",
      "@odata.etag": "W/\"CQAAABYAAAARn2vdzPFjSbaPPxzjlzOTAAASsKZz\"",
      "subject": "Holiday hours update",
      "isRead": "true",
      "sender": {
        "emailAddress": {
          "name": "Dana Swope",
          "address": "danas@contoso.onmicrosoft.com"
        }
      },
      "id": "AAMkADNkNAAASq35xAAA="
    }
  ]
}
```

## <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](delta-query-overview.md)
- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](delta-query-events.md)
- [Obter as alterações incrementais para grupos](delta-query-groups.md)
- [Obter as alterações incrementais para usuários](delta-query-users.md)
