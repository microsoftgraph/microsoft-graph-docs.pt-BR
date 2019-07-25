---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 914b1d52908cd1936b8fdf87df336ef8b2603552
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITrustFrameworkPolicyCollectionPage policies = graphClient.trustFramework().policies()
    .buildRequest()
    .get();

```