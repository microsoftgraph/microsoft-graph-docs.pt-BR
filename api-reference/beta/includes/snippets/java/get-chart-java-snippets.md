---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3784929e073cf3a95acf4aadcff651dd9599675d358259c139c2d6fae05d6eae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215414"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChart workbookChart = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .buildRequest()
    .get();

```