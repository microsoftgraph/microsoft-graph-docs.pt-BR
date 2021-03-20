---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40e34ff1f45635c43c23438a8ad15a2c2c7bca42
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967124"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartGridlines workbookChartGridlines = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().minorGridlines()
    .buildRequest()
    .get();

```