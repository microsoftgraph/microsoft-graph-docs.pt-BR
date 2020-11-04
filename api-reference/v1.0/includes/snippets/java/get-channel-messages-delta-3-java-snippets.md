---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66bf5e253f37bda3be0083f7e36aefab86a43112
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA="));

ChatMessage chatMessage = graphClient.teams("{id}").channels("{id}").messages("delta")
    .buildRequest( requestOptions )
    .get();

```