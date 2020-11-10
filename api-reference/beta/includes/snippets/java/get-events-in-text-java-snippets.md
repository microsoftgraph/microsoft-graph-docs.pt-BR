---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d74712b2696fb5397c42f5bd2216d8e16c2c18b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973563"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

IEventCollectionPage events = graphClient.me().events()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```