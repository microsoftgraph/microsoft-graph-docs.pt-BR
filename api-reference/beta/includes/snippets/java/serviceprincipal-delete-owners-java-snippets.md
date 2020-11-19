---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 72df4b83ac3549bef5847dc92cb4abba7852a093
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350446"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```