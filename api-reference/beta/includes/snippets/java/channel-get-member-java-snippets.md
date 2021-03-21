---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97659436ad8d5b9336334d9998fbb6c773fc271d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980782"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").channels("19:56eb04e133944cf69e603c5dac2d292e@thread.skype").members("ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=")
    .buildRequest()
    .get();

```