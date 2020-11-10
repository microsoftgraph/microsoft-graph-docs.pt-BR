---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6221368f4d66888631e0cbfc739534384b974c5c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationalActivityCollectionPage educationalActivities = graphClient.me().profile().educationalActivities()
    .buildRequest()
    .get();

```