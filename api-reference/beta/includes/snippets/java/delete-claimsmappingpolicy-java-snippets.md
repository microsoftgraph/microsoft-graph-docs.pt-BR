---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35d567f5f9f71f2506d7f85a0fe3a6f99657cd7e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958084"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .delete();

```