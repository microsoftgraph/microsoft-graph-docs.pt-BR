---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b82787718afb3846826d45ff6251d55e949641d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021081"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.chats("19:meeting_ZDZlYTYxOWUtYzdlMi00ZmMxLWIxMTAtN2YzODZlZjAxYzI4@thread.v2")
    .buildRequest()
    .get();

```