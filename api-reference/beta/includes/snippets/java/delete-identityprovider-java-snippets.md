---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8786f2c3e8b6db2ed81cbcfb06de645e91634ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953435"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityProviders("{id}")
    .buildRequest()
    .delete();

```