---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cff8acb874ad11b75e1ac7c7890f8e72d28807ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979104"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));

Event event = graphClient.me().events("AAMkAGI1AAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview")
    .get();

```