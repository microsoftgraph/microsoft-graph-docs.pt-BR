---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2179a2f99781209d67519923908783be68914fd6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855887"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IItemActivityOLDCollectionPage activities = graphClient.me().drive().activities()
    .buildRequest()
    .get();

```