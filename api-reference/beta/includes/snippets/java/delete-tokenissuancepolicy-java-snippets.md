---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eee5ca04d0b00eeafce73e6646377eb50b023915
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968887"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .delete();

```