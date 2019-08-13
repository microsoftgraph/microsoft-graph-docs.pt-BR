---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 313aea4aad66cd645b788f80484593b8556111fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358999"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessPeerToPeerActivityCountsCollectionPage getSkypeForBusinessPeerToPeerActivityCounts = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityCounts("D7")
    .buildRequest()
    .get();

```