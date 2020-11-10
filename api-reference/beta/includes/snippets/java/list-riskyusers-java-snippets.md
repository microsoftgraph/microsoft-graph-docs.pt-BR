---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17a8087759d63558be18805b25818634b25c2718
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979171"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserCollectionPage riskyUsers = graphClient.riskyUsers()
    .buildRequest()
    .get();

```