---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddec62a4d84998183d934a0ebd74fb0d38e83955
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983063"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageCollectionPage messages = graphClient.chats("{id}").messages()
    .buildRequest()
    .get();

```