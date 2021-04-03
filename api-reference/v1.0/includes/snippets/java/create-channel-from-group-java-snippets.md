---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7fb068d5b7192e2e27490984bed1f7b4af92407
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508435"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.displayName = "Architecture Discussion";
channel.description = "This channel is where we debate all future architecture plans";
channel.membershipType = ChannelMembershipType.STANDARD;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels()
    .buildRequest()
    .post(channel);

```