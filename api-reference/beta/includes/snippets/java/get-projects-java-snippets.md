---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af44ad19bab2a6ee7c10c1603ead5bb0f8a3bfc2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980696"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProjectParticipationCollectionPage projects = graphClient.me().profile().projects()
    .buildRequest()
    .get();

```