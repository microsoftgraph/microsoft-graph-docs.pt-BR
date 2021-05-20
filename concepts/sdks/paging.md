---
title: Page through a collection using the Microsoft Graph SDKs
description: Fornece instruções para criar solicitações Graph API da Microsoft usando os SDKs do Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d06a23e5c1e53042192fe3fe8b4c8e3fe13c488d
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579659"
---
# <a name="page-through-a-collection-using-the-microsoft-graph-sdks"></a><span data-ttu-id="bd062-103">Page through a collection using the Microsoft Graph SDKs</span><span class="sxs-lookup"><span data-stu-id="bd062-103">Page through a collection using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="bd062-104">Por motivos de desempenho, as coleções de entidades geralmente são divididas em páginas e cada página é retornada com uma URL para a próxima página.</span><span class="sxs-lookup"><span data-stu-id="bd062-104">For performance reasons, collections of entities are often split into pages and each page is returned with a URL to the next page.</span></span> <span data-ttu-id="bd062-105">A **classe PageIterator** simplifica o consumo de coleções pagedas.</span><span class="sxs-lookup"><span data-stu-id="bd062-105">The **PageIterator** class simplifies consuming of paged collections.</span></span> <span data-ttu-id="bd062-106">**PageIterator** lida com a enumeração da página atual e solicita páginas subsequentes automaticamente.</span><span class="sxs-lookup"><span data-stu-id="bd062-106">**PageIterator** handles enumerating the current page and requesting subsequent pages automatically.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd062-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd062-107">Request headers</span></span>

<span data-ttu-id="bd062-108">Se você enviar quaisquer headers de solicitação adicionais em sua solicitação inicial, esses headers não serão incluídos por padrão nas solicitações de página subsequentes.</span><span class="sxs-lookup"><span data-stu-id="bd062-108">If you send any additional request headers in your initial request, those headers are not included by default in subsequent page requests.</span></span> <span data-ttu-id="bd062-109">Se esses headers precisam ser enviados em solicitações subsequentes, você deve defini-los explicitamente.</span><span class="sxs-lookup"><span data-stu-id="bd062-109">If those headers need to be sent on subsequent requests, you must set them explicitly.</span></span>

## <a name="iterate-over-all-the-messages"></a><span data-ttu-id="bd062-110">Iterar sobre todas as mensagens</span><span class="sxs-lookup"><span data-stu-id="bd062-110">Iterate over all the messages</span></span>

<span data-ttu-id="bd062-111">O exemplo a seguir mostra iteração sobre todas as mensagens na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bd062-111">The following example shows iterating over all the messages in a user's mailbox.</span></span>

> [!TIP]
> <span data-ttu-id="bd062-112">Este exemplo define um pequeno tamanho de página usando `top` o parâmetro para fins de demonstração.</span><span class="sxs-lookup"><span data-stu-id="bd062-112">This example sets a small page size using the `top` parameter for demonstration purposes.</span></span> <span data-ttu-id="bd062-113">Você pode definir o tamanho da página até 999 para minimizar o número de solicitações necessárias.</span><span class="sxs-lookup"><span data-stu-id="bd062-113">You can set the page size up to 999 to minimize the number of requests that are necessary.</span></span>

### <a name="c"></a>[<span data-ttu-id="bd062-114">C#</span><span class="sxs-lookup"><span data-stu-id="bd062-114">C#</span></span>](#tab/csharp)

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

### <a name="typescript"></a>[<span data-ttu-id="bd062-115">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd062-115">TypeScript</span></span>](#tab/typeScript)

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

### <a name="java"></a>[<span data-ttu-id="bd062-116">Java</span><span class="sxs-lookup"><span data-stu-id="bd062-116">Java</span></span>](#tab/java)

```java
final MessageCollectionPage messagesPage = graphClient.me().messages()
    .buildRequest(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""))
    .select("Sender,Subject,Body")
    .top(10)
    .get();


while(messagesPage != null) {
  final List<Message> messages = messagesPage.getCurrentPage();
  final MessageCollectionRequestBuilder nextPage = messagesPage.getNextPage();
  if(nextPage == null) {
    break;
  } else {
    messagePage = nextPage.buildRequest(
        // Re-add the header to subsequent requests
        new HeaderOption("Prefer", "outlook.body-content-type=\"text\"")
    ).get();
  }
}
```

---

## <a name="stopping-and-resuming-the-iteration"></a><span data-ttu-id="bd062-117">Parar e retomar a iteração</span><span class="sxs-lookup"><span data-stu-id="bd062-117">Stopping and resuming the iteration</span></span>

<span data-ttu-id="bd062-118">Alguns cenários exigem parar o processo de iteração para executar outras ações.</span><span class="sxs-lookup"><span data-stu-id="bd062-118">Some scenarios require stopping the iteration process in order to perform other actions.</span></span> <span data-ttu-id="bd062-119">É possível pausar a iteração retornando do `false` retorno de chamada de iteração.</span><span class="sxs-lookup"><span data-stu-id="bd062-119">It is possible to pause the iteration by returning `false` from the iteration callback.</span></span> <span data-ttu-id="bd062-120">A iteração pode ser retomada chamando o `resume` método no **PageIterator**.</span><span class="sxs-lookup"><span data-stu-id="bd062-120">Iteration can be resumed by calling the `resume` method on the **PageIterator**.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="bd062-121">C#</span><span class="sxs-lookup"><span data-stu-id="bd062-121">C#</span></span>](#tab/csharp)

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
    Thread.Sleep(5000);
    // Reset count
    count = 0;
    await pageIterator.ResumeAsync();
}
```

### <a name="typescript"></a>[<span data-ttu-id="bd062-122">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd062-122">TypeScript</span></span>](#tab/typeScript)

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

### <a name="java"></a>[<span data-ttu-id="bd062-123">Java</span><span class="sxs-lookup"><span data-stu-id="bd062-123">Java</span></span>](#tab/java)

```java
// not supported in java SDK
```

---
<!-- markdownlint-enable MD024 -->
