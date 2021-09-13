---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: addc674f5143d674ecb2d4dfc91a174a310807640b1b0a2032f75190006fe4b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReply(MessageCreateReplyParameterSet
        .newBuilder()
        .withMessage(null)
        .withComment(null)
        .build())
    .buildRequest()
    .post();

```