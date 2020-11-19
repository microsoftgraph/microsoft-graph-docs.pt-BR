---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: cb826ed9762e698ad79b075245562ac69a3501ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222162"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19")
    .acceptRecommendations()
    .buildRequest()
    .post();

```