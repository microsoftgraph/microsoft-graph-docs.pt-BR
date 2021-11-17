---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f3a1bcc05e4da0a4129b2ed69fbcabaa5984dfdbb2276e38c5fe69e8483f14c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160234"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> messageIdsList = new LinkedList<String>();
messageIdsList.add("MC172851");
messageIdsList.add("MC167983");

graphClient.admin().serviceAnnouncement().messages()
    .unfavorite(ServiceUpdateMessageUnfavoriteParameterSet
        .newBuilder()
        .withMessageIds(messageIdsList)
        .build())
    .buildRequest()
    .post();

```