---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d836aae79138b22818e7c93624ecab49b4aa4ffa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomListCollectionPage roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```