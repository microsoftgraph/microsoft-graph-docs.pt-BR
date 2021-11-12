---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f17bb31175c8118ef38644cdc3cda64ebb6f99de5c08317399df9c91555981b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159375"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTask outlookTask = new OutlookTask();
outlookTask.subject = "Shop for dinner";
DateTimeTimeZone startDateTime = new DateTimeTimeZone();
startDateTime.dateTime = "2016-04-23T18:00:00";
startDateTime.timeZone = "Pacific Standard Time";
outlookTask.startDateTime = startDateTime;
DateTimeTimeZone dueDateTime = new DateTimeTimeZone();
dueDateTime.dateTime = "2016-04-25T13:00:00";
dueDateTime.timeZone = "Pacific Standard Time";
outlookTask.dueDateTime = dueDateTime;

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPXAAA=").tasks()
    .buildRequest()
    .post(outlookTask);

```