---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9bd4a9565f99d8547b73fa6f72ecc4f6f863fdd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961204"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .get();

```