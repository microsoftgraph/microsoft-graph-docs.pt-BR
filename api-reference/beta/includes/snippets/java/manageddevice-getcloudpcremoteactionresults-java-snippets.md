---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aaabe157da80f13e3e34d45eff920ce0a016c318
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59766782"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceGetCloudPcRemoteActionResultsCollectionPage getCloudPcRemoteActionResults = graphClient.deviceManagement().managedDevices("{managedDeviceId}")
    .getCloudPcRemoteActionResults()
    .buildRequest()
    .get();

```