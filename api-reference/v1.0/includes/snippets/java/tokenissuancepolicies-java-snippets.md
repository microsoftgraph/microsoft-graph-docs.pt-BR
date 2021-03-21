---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f90fa8eddd51c126697adf610837b6421d701dc1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicyCollectionPage tokenIssuancePolicies = graphClient.policies().tokenIssuancePolicies()
    .buildRequest()
    .get();

```