---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64fd03aa16c8b363eaca32c8a72074ded46d54ec
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcReviewStatus cloudPcReviewStatus = graphClient.deviceManagement().managedDevices("185f01c2de954929afb129392e5d9f47")
    .getCloudPcReviewStatus()
    .buildRequest()
    .get();

```