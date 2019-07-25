---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52eb02cec60894c17fa9676c6441a2a7ac4ab777
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860014"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .reset()
    .buildRequest()
    .post();

```