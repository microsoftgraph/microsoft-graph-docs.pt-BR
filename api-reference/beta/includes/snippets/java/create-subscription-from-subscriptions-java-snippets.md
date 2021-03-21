---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 632c25635c61c1248fea4797ffee892e8e6f87a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981587"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "created";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = OffsetDateTimeSerializer.deserialize("2016-11-20T18:23:45.9356913Z");
subscription.clientState = "secretClientValue";
subscription.latestSupportedTlsVersion = "v1_2";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```