---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e82accc561d61fa874d5eb47c41cfa63d5850cf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979863"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Message message = graphClient.me().messages("AAMkAGI1AAAoZCfHAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,uniqueBody")
    .get();

```