---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 673c8dc00b3318a82d59179858ef1355420a22b2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983160"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "Shared legal agreements";

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .patch(driveItem);

```