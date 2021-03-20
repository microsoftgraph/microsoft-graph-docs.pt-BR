---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3b5c962e620a2977420a15897492d03b1dfb73c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityStatisticsCollectionPage activityStatistics = graphClient.me().analytics().activityStatistics()
    .buildRequest()
    .get();

```