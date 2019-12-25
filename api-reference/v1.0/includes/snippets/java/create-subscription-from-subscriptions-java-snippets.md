---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b618cd8b5f2cb9ec84c2ea1f57086ff7b6d526f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864115"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "updated";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = "2016-11-20T18:23:45.9356913Z";
subscription.clientState = "secretClientValue";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```