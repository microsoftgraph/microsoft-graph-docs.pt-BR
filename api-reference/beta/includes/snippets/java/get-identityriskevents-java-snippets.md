---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95f738d45317cda592d5a170d8329c3865f08a8c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857552"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityRiskEventCollectionPage identityRiskEvents = graphClient.identityRiskEvents()
    .buildRequest()
    .get();

```