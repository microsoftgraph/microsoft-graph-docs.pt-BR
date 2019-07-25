---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa07909e7dc109f9e39c36653d75de42e6d4451e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867192"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

IMessageCollectionPage messages = graphClient.me().messages()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,uniqueBody")
    .get();

```