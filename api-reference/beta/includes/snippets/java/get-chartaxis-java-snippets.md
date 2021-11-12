---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7baf8ef2fba62126b61911486a72e6c170bd54f6bc551ab8469a118ed0913816
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899101"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxis workbookChartAxis = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis()
    .buildRequest()
    .get();

```