---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b87d882b906e7e45e2fccae0600baed6a48d342b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr").items("TSP228082938")
    .buildRequest()
    .delete();

```