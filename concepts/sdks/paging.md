---
title: Page through a collection using the Microsoft Graph SDKs
description: Fornece instruções para criar solicitações Graph API da Microsoft usando os SDKs do Microsoft Graph.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: a6ccc53fd58685948c486ff047733ba88949e553
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560040"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a>Page through a collection using the Microsoft Graph SDKs

Por motivos de desempenho, as coleções de entidades geralmente são divididas em páginas e cada página é retornada com uma URL para a próxima página. A **classe PageIterator** simplifica o consumo de coleções pagedas. **PageIterator** lida com a enumeração da página atual e solicita páginas subsequentes automaticamente.

## <a name="request-headers"></a>Cabeçalhos de solicitação

Se você enviar quaisquer headers de solicitação adicionais em sua solicitação inicial, esses headers não serão incluídos por padrão nas solicitações de página subsequentes. Se esses cabeçalhos precisam ser enviados em solicitações subsequentes, você deve defini-los explicitamente.

## <a name="iterate-over-all-the-messages"></a>Iterar sobre todas as mensagens

O exemplo a seguir mostra iteração sobre todas as mensagens na caixa de correio de um usuário.

> [!TIP]
> Este exemplo define um pequeno tamanho de página usando o `top` parâmetro para fins de demonstração. Você pode definir o tamanho da página até 999 para minimizar o número de solicitações necessárias.

### <a name="c"></a>[C#](#tab/csharp)

```csharp
var messages = await graphClient.Me.Messages
    .Request()
    .Header("Prefer", "outlook.body-content-type=\"text\"")
    .Select(e => new {
        e.Sender,
        e.Subject,
        e.Body
    })
    .Top(10)
    .GetAsync();

var pageIterator = PageIterator<Message>
    .CreatePageIterator(
        graphClient,
        messages,
        // Callback executed for each item in
        // the collection
        (m) =>
        {
            Console.WriteLine(m.Subject);
            return true;
        },
        // Used to configure subsequent page
        // requests
        (req) =>
        {
            // Re-add the header to subsequent requests
            req.Header("Prefer", "outlook.body-content-type=\"text\"");
            return req;
        }
    );

await pageIterator.IterateAsync();
```

### <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
// Makes request to fetch mails list.
let response: PageCollection = await client
  .api("/me/messages?$top=10&$select=sender,subject,body")
  .header('Prefer', 'outlook.body-content-type="text"')
  .get();

// A callback function to be called for every item in the collection.
// This call back should return boolean indicating whether not to
// continue the iteration process.
let callback: PageIteratorCallback = (data) => {
  console.log(data.subject);
  return true;
};

// A set of request options to be applied to
// all subsequent page requests
let requestOptions: GraphRequestOptions = {
  // Re-add the header to subsequent requests
  headers: {
    'Prefer': 'outlook.body-content-type="text"'
  }
};

// Creating a new page iterator instance with client a graph client
// instance, page collection response from request and callback
let pageIterator = new PageIterator(client, response, callback, requestOptions);

// This iterates the collection until the nextLink is drained out.
await pageIterator.iterate();
```

### <a name="java"></a>[Java](#tab/java)

```java
MessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""))
    .select("Sender,Subject,Body")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.getCurrentPage();
  final MessageCollectionRequestBuilder nextPage = messagesPage.getNextPage();
  if (nextPage == null) {
    break;
  } else {
    messagesPage = nextPage.buildRequest(
        // Re-add the header to subsequent requests
        new HeaderOption("Prefer", "outlook.body-content-type=\"text\"")
    ).get();
  }
}
```

### <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    msgraphcore "github.com/microsoftgraph/msgraph-sdk-go-core"
    "github.com/microsoftgraph/msgraph-sdk-go/me/messages"
    "github.com/microsoftgraph/msgraph-sdk-go/models/microsoft/graph"
)

query := messages.MessagesRequestBuilderGetQueryParameters{
    Select: []string{"body", "sender", "subject"},
}

options := messages.MessagesRequestBuilderGetOptions{
    H: map[string]string{
        "Prefer": "outlook.body-content-type=\"text\"",
    },
    Q: &query,
}

result, err := client.Me().Messages().Get(&options)

// Initialize iterator
pageIterator, err := msgraphcore.NewPageIterator(result, adapter, graph.CreateMessageCollectionResponseFromDiscriminatorValue)

// Any custom headers sent in original request should also be added
// to the iterator
pageIterator.SetHeaders(options.H)

// Iterate over all pages
iterateErr := pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    fmt.Printf("%s\n", *message.GetSubject())
    // Return true to continue the iteration
    return true
})
```

---

## <a name="stopping-and-resuming-the-iteration"></a>Parar e retomar a iteração

Alguns cenários exigem parar o processo de iteração para executar outras ações. É possível pausar a iteração retornando `false` do retorno de chamada de iteração. A iteração pode ser retomada chamando o método `resume` no **PageIterator**.

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
    .CreatePageIterator(
        graphClient,
        messages,
        (m) =>
        {
            Console.WriteLine(m.Subject);
            count++;
            // If we've iterated over the limit,
            // stop the iteration by returning false
            return count < pauseAfter;
        }
    );

await pageIterator.IterateAsync();

while (pageIterator.State != PagingState.Complete)
{
    Console.WriteLine("Iteration paused for 5 seconds...");
    await Task.Delay(5000);
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

### <a name="java"></a>[Java](#tab/java)

```java
// not supported in java SDK
```

### <a name="go"></a>[Ir](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    msgraphcore "github.com/microsoftgraph/msgraph-sdk-go-core"
    "github.com/microsoftgraph/msgraph-sdk-go/me/messages"
    "github.com/microsoftgraph/msgraph-sdk-go/models/microsoft/graph"
)

query := messages.MessagesRequestBuilderGetQueryParameters{
    Select: []string{"body", "sender", "subject"},
}

options := messages.MessagesRequestBuilderGetOptions{
    H: map[string]string{
        "Prefer": "outlook.body-content-type=\"text\"",
    },
    Q: &query,
}

result, err := client.Me().Messages().Get(&options)

// Initialize iterator
pageIterator, err := msgraphcore.NewPageIterator(result, adapter, graph.CreateMessageCollectionResponseFromDiscriminatorValue)

// Any custom headers sent in original request should also be added
// to the iterator
pageIterator.SetHeaders(options.H)

// Pause iterating after 25
var count, pauseAfter = 0, 25

// Iterate over all pages
iterateErr := pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    count++
    fmt.Printf("%d: %s\n", count, *message.GetSubject())
    // Once count = 25, this returns false,
    // Which pauses the iteration
    return count < pauseAfter
})

// Pause 5 seconds
fmt.Printf("Iterated first %d messages, pausing for 5 seconds...\n", pauseAfter)
time.Sleep(5 * time.Second)
fmt.Printf("Resuming iteration...\n")

// Resume iteration
iterateErr = pageIterator.Iterate(func(pageItem interface{}) bool {
    message := pageItem.(graph.Message)
    count++
    fmt.Printf("%d: %s\n", count, *message.GetSubject())
    // Return true to continue the iteration
    return true
})
```

---
<!-- markdownlint-enable MD024 -->
