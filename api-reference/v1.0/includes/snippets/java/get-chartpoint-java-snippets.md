---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3655429ffc1e41805d8ad156ecb20ae182c883bf895d9697885c3d1c878a333f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{series-id}").points("{point-id}")
    .buildRequest()
    .get();

```