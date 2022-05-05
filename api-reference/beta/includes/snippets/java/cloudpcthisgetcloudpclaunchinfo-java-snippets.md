---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 724667979a469b312610a50e093af6870707159b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcLaunchInfo cloudPcLaunchInfo = graphClient.me().cloudPCs("{cloudPCId}")
    .getCloudPcLaunchInfo()
    .buildRequest()
    .get();

```