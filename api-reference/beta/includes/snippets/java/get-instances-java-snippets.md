---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62711d6a67db1208272cab1ef2a89ac901b4f98b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967467"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2019-04-08T09:00:00.0000000"));
requestOptions.add(new QueryOption("endDateTime", "2019-04-30T09:00:00.0000000"));

EventCollectionPage instances = graphClient.me().events("AAMkAGUzYRgWAAA=").instances()
    .buildRequest( requestOptions )
    .select("subject,bodyPreview,seriesMasterId,type,recurrence,start,end")
    .get();

```