---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dccdb97766bb097fa6e252e389561ccaf9ce53f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973632"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookRangeBorderCollectionPage borders = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders()
    .buildRequest()
    .get();

```