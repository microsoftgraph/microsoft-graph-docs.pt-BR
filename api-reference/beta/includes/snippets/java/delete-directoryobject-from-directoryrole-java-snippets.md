---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7919fa4ae2f595ab3db2b80b2b5227d3133289ea
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962944"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryRoles("{id}").members("{id}").reference()
    .buildRequest()
    .delete();

```