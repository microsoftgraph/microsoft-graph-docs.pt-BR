---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74043dfb0b802e3b97fc692e23b69d04a80ccbf0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965661"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr")
    .buildRequest()
    .delete();

```