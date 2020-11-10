---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47c680f428ab1514a97d0843166d8a1fb0f457c1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958024"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .get();

```