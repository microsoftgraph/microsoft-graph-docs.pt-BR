---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06cc43d95cb38a4fc243eb33f7b874565de02354
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971644"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage favoritePlans = graphClient.me().planner().favoritePlans()
    .buildRequest()
    .get();

```