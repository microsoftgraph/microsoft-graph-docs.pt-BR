---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44e73537abdd733aed7f97a69650204b0bb302fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

Event event = graphClient.me().events("AAMkAGIAAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees")
    .get();

```