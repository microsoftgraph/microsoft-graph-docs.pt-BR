---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76c791feb242e11b82fa3fa3206e8051626291ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968851"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonCollectionPage people = graphClient.me().people()
    .buildRequest()
    .get();

```