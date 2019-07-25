---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52e432faf3257384f61ccfd47c56bab10460068e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884910"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow()
    .buildRequest()
    .get();

```