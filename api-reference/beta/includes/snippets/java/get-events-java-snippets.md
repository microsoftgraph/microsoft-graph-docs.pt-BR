---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 057bc8b182f87db117196d14bec4d7fa5e5394cef2a8f132fbd35e8367334856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

EventCollectionPage events = graphClient.me().events()
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location")
    .get();

```