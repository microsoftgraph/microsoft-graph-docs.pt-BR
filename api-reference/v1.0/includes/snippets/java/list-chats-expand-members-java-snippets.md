---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4890b34c216644b4574466210a0d45cf079f1981
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038318"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .expand("members")
    .get();

```