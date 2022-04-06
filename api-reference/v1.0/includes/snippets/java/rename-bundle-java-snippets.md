---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 673c8dc00b3318a82d59179858ef1355420a22b2
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758045"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "Shared legal agreements";

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .patch(driveItem);

```