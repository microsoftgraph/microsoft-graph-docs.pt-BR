---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d570828a5059c06358532de2e428d8a6cf8420c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeriesCollectionPage series = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series()
    .buildRequest()
    .get();

```