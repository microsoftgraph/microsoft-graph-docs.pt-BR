---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 838b6d2b33b5f9ad949290f62434053bec277195
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Eastern Standard Time\""));

OutlookTask outlookTask = new OutlookTask();
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-05-06T16:00:00";
dueDateTime.timeZone = "Eastern Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().tasks("AAMkADA1MTHgwAAA=")
    .buildRequest( requestOptions )
    .patch(outlookTask);

```