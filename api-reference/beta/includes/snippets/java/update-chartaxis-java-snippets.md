---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe496b44cc461dd5d26b5e82dd28900162ea789dbe04a50e6ec33a5df16e3b98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216618"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxis workbookChartAxis = new WorkbookChartAxis();
JsonElement majorUnit = new JsonObject();
workbookChartAxis.majorUnit = majorUnit;
JsonElement maximum = new JsonObject();
workbookChartAxis.maximum = maximum;
JsonElement minimum = new JsonObject();
workbookChartAxis.minimum = minimum;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis()
    .buildRequest()
    .patch(workbookChartAxis);

```