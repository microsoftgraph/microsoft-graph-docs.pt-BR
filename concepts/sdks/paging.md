---
title: Página por meio de uma coleção usando os SDKs do Microsoft Graph
description: Fornece instruções para criar solicitações de API do Microsoft Graph usando os SDKs do Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: e3cd656c5210739436ff9df68cfb700f264204de
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "44052516"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>Página por meio de uma coleção usando os SDKs do Microsoft Graph

Por motivos de desempenho, as coleções de entidades são freqüentemente divididas em páginas e cada página é retornada com uma URL para a próxima página. A classe **PageIterator** simplifica o consumo de coleções paginadas. **PageIterator** Handles enumerando a página atual e solicitando páginas subsequentes automaticamente.

## <a name="iterate-over-all-the-messages"></a>Iterar em todas as mensagens

O exemplo a seguir mostra a iteração em todas as mensagens na caixa de correio de um usuário.

> [!TIP]
> Este exemplo define um tamanho de página pequeno usando `top` o parâmetro para fins de demonstração. Você pode definir o tamanho da página até 999 para minimizar o número de solicitações necessárias.

### <a name="c"></a>[C#](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        return true;
    });

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject")
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

---

## <a name="stopping-and-resuming-the-iteration"></a>Interromper e retomar a iteração

Alguns cenários exigem a interrupção do processo de iteração para executar outras ações. É possível pausar a iteração retornando `false` do retorno de chamada de iteração. A iteração pode ser retomada `resume` chamando-se o método no **PageIterator**.

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
int count = 0;
int pauseAfter = 25;

var messages = await graphClient.Me.Messages
    .Request()
    .Select(e => new {
        e.Sender,
        e.Subject
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(graphClient, messages, (m) => {
        Console.WriteLine(m.Subject);
        count++;
        // If we've iterated over the limit,
        // stop the iteration by returning false
        return count < pauseAfter;
    });

await pageIterator.IterateAsync();

while (pageIterator.State != PagingState.Complete)
{
    Console.WriteLine("Iteration paused for 5 seconds...");
    Thread.Sleep(5000);
    // Reset count
    count = 0;
    await pageIterator.ResumeAsync();
}
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
let count: number = 0;
let pauseAfter: number = 25;

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();

let callback: PageIteratorCallback = (data) => {
  result = `${result}${data.subject}\n`;
  console.log(data.subject);
  count++;

  // If we've iterated over the limit,
  // stop the iteration by returning false
  return count < pauseAfter;
};

let pageIterator = new PageIterator(client, response, callback);
await pageIterator.iterate();

while (!pageIterator.isComplete()) {
  console.log('Iteration paused for 5 seconds...');
  await new Promise(resolve => setTimeout(resolve, 5000));

  // Reset count
  count = 0;
  await pageIterator.resume();
}
```

---
<!-- markdownlint-enable MD024 -->
