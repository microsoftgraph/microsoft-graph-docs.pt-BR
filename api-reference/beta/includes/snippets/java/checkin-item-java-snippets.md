---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6d2dbb340ffbae4834fadad455507b80abda9cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Updating the latest guidelines";

graphClient.drives("{drive-id}").items("{item-id}")
    .checkin(DriveItemCheckinParameterSet
        .newBuilder()
        .withCheckInAs(null)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```