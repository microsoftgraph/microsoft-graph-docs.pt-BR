---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bcb904ec0486ed4db9834c44fb4304ac5624050
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range('A1:B2')
    .buildRequest()
    .get();

```