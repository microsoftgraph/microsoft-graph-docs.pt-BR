---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d0c41b38808689da26d25c6f8baa7e859999040
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLegend workbookChartLegend = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").legend()
    .buildRequest()
    .get();

```