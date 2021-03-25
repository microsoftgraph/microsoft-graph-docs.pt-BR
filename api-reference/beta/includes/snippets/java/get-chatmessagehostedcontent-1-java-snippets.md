---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 648466ed577915c6ea35cccae6ef33c13ecd4d92
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContent chatMessageHostedContent = graphClient.chats("{id}").messages("{id}").hostedContents("{id}")
    .buildRequest()
    .get();

```