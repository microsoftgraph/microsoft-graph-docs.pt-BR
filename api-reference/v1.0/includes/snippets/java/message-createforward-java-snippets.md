---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e6bec70abe14a1b014d89df293cba54d00a2a1762b26cc027b015d77c8cbe26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createForward(MessageCreateForwardParameterSet
        .newBuilder()
        .withToRecipients(null)
        .withMessage(null)
        .withComment(null)
        .build())
    .buildRequest()
    .post();

```