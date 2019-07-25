---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8683e0f7ef0cf356ca9067e986c89f3503a77683
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870168"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IServicePrincipalDeltaCollectionPage delta = graphClient.servicePrincipals()
    .delta()
    .buildRequest()
    .get();

```