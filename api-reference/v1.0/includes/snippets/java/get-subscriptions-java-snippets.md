---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02b12041affc9e9a7ec9cd1ee418ba706a6814b538c7371d79bf8276f53ecebf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214269"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscriptionCollectionPage subscriptions = graphClient.subscriptions()
    .buildRequest()
    .get();

```