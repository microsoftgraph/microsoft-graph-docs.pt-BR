---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 018baa300d523f6f75252e9d848adce27b93755a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952497"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IActivityStatisticsCollectionPage activityStatistics = graphClient.me().analytics().activityStatistics()
    .buildRequest()
    .get();

```