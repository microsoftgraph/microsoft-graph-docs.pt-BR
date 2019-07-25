---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfcb82f8f054cbca18307633c08b3160f3fdabb8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872808"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityPagesCollectionPage getSharePointActivityPages = graphClient.reports()
    .getSharePointActivityPages('D7')
    .buildRequest()
    .get();

```