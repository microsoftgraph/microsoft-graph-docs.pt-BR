---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebf5f5967b63ba84dacab30386df4be817ef145c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881221"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTable workbookPivotTable = graphClient.me().drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .buildRequest()
    .get();

```