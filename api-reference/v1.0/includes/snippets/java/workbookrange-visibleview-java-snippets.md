---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59f8890836b719b0f3491097e6ed056f1c1ad8e8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884868"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeView workbookRangeView = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range('A1:Z10')
    .visibleView()
    .buildRequest()
    .get();

```