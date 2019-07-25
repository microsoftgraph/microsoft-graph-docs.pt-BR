---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec629d20a20cd247e5b9f01ba9766247c2532719
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888389"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAnalytics itemAnalytics = graphClient.drives("{drive-id}").items("{item-id}").analytics()
    .buildRequest()
    .get();

```