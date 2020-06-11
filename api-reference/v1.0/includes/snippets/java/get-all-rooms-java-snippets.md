---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48fa44fb125641be1883c9813728fa3600583e67
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685226"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomCollectionPage room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```