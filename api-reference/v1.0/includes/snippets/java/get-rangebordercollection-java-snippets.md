---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dccdb97766bb097fa6e252e389561ccaf9ce53f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookRangeBorderCollectionPage borders = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders()
    .buildRequest()
    .get();

```