---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0a9f68cd91686cee6b774c80f5edb0fc3196384
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884240"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .usedRange()
    .buildRequest()
    .get();

```