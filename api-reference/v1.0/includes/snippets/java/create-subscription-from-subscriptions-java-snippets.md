---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f72f6fac70da465092c73acfb22b36d2b77db26a
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41956442"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "updated";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = "2016-11-20T18:23:45.9356913Z";
subscription.clientState = "secretClientValue";
subscription.latestSupportedTlsVersion = "v1_2";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```