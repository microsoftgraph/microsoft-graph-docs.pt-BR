---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb0e97027d9e8ce55fbfd4c0f4ed4f6f8c05487f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961313"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LongRunningOperation longRunningOperation = graphClient.users("{id | userPrincipalName}").authentication().operations("{id}")
    .buildRequest()
    .get();

```