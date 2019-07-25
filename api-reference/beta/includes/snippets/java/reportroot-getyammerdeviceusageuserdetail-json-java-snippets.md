---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e15c665d1efa156b3ef0f472dfd6931a6bf848e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871498"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IYammerDeviceUsageUserDetailCollectionPage getYammerDeviceUsageUserDetail = graphClient.reports()
    .getYammerDeviceUsageUserDetail('D7')
    .buildRequest()
    .get();

```