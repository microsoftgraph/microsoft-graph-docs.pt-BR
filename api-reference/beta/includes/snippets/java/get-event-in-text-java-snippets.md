---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a192cd1654df33c9959ce2207bea1f653217cf48
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954869"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Event event = graphClient.me().events("AAMkAGI1AAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```