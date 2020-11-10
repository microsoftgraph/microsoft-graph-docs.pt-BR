---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c111862dc92fa23d655a8504b293a1f240a909a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951793"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .buildRequest()
    .delete();

```