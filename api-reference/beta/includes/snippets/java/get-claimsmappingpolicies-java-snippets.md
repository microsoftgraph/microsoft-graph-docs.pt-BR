---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf11154d3f1e7c675bba937bdfc8324b5be90a82
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958003"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IClaimsMappingPolicyCollectionPage claimsMappingPolicies = graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .get();

```