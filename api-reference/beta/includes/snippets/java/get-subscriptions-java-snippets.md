---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51b7679c6222227c510d57512c5f538b3d33e8d1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscriptionCollectionPage subscriptions = graphClient.subscriptions()
    .buildRequest()
    .get();

```