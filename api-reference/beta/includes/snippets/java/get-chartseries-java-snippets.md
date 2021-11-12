---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79eca3c71e16fae6a6144e4f8f7d3c1c4a58ccc1ff3584bf2ffe23d7bd1befc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}")
    .buildRequest()
    .get();

```