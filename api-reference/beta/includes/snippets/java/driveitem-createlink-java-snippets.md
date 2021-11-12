---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08b7b446f8f455cd5a00a7985b0cae1795cb807c354bf2bff0a6e03cd20a3419
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273717"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String scope = "anonymous";

String password = "String";

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();

recipientsList.add(recipients);

graphClient.me().drive().items("{itemId}")
    .createLink(DriveItemCreateLinkParameterSet
        .newBuilder()
        .withType(type)
        .withScope(scope)
        .withExpirationDateTime(null)
        .withPassword(password)
        .withMessage(null)
        .withRecipients(recipientsList)
        .build())
    .buildRequest()
    .post();

```