---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2bdbeb8977f36e3757e01e68bef9deda0c3335c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974264"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}")
    .buildRequest()
    .get();

```