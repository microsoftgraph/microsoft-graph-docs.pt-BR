---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64e917e0531c115ac281cd4f320c0d1be776246e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855298"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationDeltaCollectionPage delta = graphClient.applications()
    .delta()
    .buildRequest()
    .get();

```