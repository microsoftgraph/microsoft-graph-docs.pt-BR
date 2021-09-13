---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01d303b03c39660f3588132a954778e8ac8b7ef2d2bcbf5cc3c485255e46ecc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407705"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = new WorkbookChartPoint();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}").points()
    .buildRequest()
    .post(workbookChartPoint);

```