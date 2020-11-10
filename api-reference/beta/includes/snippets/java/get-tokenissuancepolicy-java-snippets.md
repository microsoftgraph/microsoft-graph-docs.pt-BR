---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2060f79b0c23dc78442f7e65fa4455241c60da8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968873"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .get();

```